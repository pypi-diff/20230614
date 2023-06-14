# Comparing `tmp/spacy-llm-0.2.1.tar.gz` & `tmp/spacy-llm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.2.1.tar", last modified: Mon Jun  5 14:11:25 2023, max compression
+gzip compressed data, was "spacy-llm-0.3.0.tar", last modified: Wed Jun 14 09:34:09 2023, max compression
```

## Comparing `spacy-llm-0.2.1.tar` & `spacy-llm-0.3.0.tar`

### file list

```diff
@@ -1,132 +1,151 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    52005 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    50761 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      698 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1819 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.439660 spacy-llm-0.2.1/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      187 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.443660 spacy-llm-0.2.1/spacy_llm/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.443660 spacy-llm-0.2.1/spacy_llm/backends/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)      328 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1233 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3788 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2791 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2574 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/integration/minichain.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.447660 spacy-llm-0.2.1/spacy_llm/backends/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)       63 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.447660 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/
--rw-r--r--   0 vsts      (1001) docker     (122)      239 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/backend/openai.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1721 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/backends/rest/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.447660 spacy-llm-0.2.1/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6937 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.447660 spacy-llm-0.2.1/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.451660 spacy-llm-0.2.1/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      534 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4525 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4282 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4490 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/spancat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.455660 spacy-llm-0.2.1/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/ner.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/rel.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/spancat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     8673 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.455660 spacy-llm-0.2.1/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/util/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4104 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tasks/util/span.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.455660 spacy-llm-0.2.1/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.459660 spacy-llm-0.2.1/spacy_llm/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/test_minichain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/backends/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)      110 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)      836 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.459660 spacy-llm-0.2.1/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4703 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.459660 spacy-llm-0.2.1/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/ner_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/ner_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/ner_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/rel_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/templates/ner_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/templates/textcat_template.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)    19490 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2690 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15057 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20909 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5926 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7848 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1727 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.443660 spacy-llm-0.2.1/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    52005 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3915 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      158 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-05 14:11:25.000000 spacy-llm-0.2.1/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.467661 spacy-llm-0.2.1/usage_examples/ner_minichain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_minichain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/ner_minichain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3508 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:11:25.475661 spacy-llm-0.2.1/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-05 14:11:15.000000 spacy-llm-0.2.1/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.634001 spacy-llm-0.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    62271 2023-06-14 09:34:09.634001 spacy-llm-0.3.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    61027 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      698 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1810 2023-06-14 09:34:09.634001 spacy-llm-0.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.618001 spacy-llm-0.3.0/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      234 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)      348 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)      502 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      279 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4712 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2583 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3435 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4715 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/hf/stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/
+-rw-r--r--   0 vsts      (1001) docker     (122)      280 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1256 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/integration/remote/minichain.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/backends/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4784 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6223 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4157 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      571 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6601 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/openai.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1901 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/backends/rest/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1033 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10806 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1702 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3959 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8011 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7790 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8788 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/spancat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/lemma.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)    15017 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      220 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      223 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4009 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4722 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tasks/util/span.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2294 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1682 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      618 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_minichain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1869 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3307 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/backends/test_stablelm.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.626001 spacy-llm-0.3.0/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6951 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/lemma_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/ner_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/ner_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/ner_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/rel_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/templates/lemma_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/templates/ner_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/templates/textcat_template.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)     7949 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21901 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5203 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16700 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23397 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5934 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2001 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8724 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.622001 spacy-llm-0.3.0/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    62271 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4685 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      149 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-06-14 09:34:09.000000 spacy-llm-0.3.0/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/ner_minichain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_minichain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/ner_minichain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.630001 spacy-llm-0.3.0/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3509 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-14 09:34:09.634001 spacy-llm-0.3.0/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-06-14 09:33:30.000000 spacy-llm-0.3.0/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.2.1/LICENSE` & `spacy-llm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/PKG-INFO` & `spacy-llm-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.2.1
+Version: 0.3.0
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -134,15 +134,15 @@
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
 labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
 [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1"
+@llm_backends = "spacy.Dolly_HF.v1"
 # For better performance, use databricks/dolly-v2-12b instead
 model = "databricks/dolly-v2-3b"
 ```
 
 Now run:
 
 ```python
@@ -230,26 +230,105 @@
 # config.cfg (excerpt)
 [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1"
 labels = LABEL1,LABEL2,LABEL3
 my_other_config_val = 0.3
 ```
 
+## Logging
+
+spacy-llm has a built-in logger that can log the prompt sent to the LLM as well as its raw response. This logger uses the debug level and by default has a `logging.NullHandler()` configured.
+
+In order to use this logger, you can setup a simple handler like this:
+
+```python
+import logging
+import spacy_llm
+
+
+spacy_llm.logger.addHandler(logging.StreamHandler())
+spacy_llm.logger.setLevel(logging.DEBUG)
+```
+
+> NOTE: Any `logging` handler will work here so you probably want to use some sort of rotating `FileHandler` as the generated prompts can be quite long, especially for tasks with few-shot examples.
+
+
+Then when using the pipeline you'll be able to view the prompt and response.
+
+E.g. with the config and code from [Example 1](##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
+
+
+```python
+from spacy_llm.util import assemble
+
+
+nlp = assemble("config.cfg")
+doc = nlp("You look gorgeous!")
+print(doc.cats)
+```
+
+You will see `logging` output similar to:
+
+```
+Generated prompt for doc: You look gorgeous!
+
+You are an expert Text Classification system. Your task is to accept Text as input
+and provide a category for the text based on the predefined labels.
+
+Classify the text below to any of the following labels: COMPLIMENT, INSULT
+The task is non-exclusive, so you can provide more than one label as long as
+they're comma-delimited. For example: Label1, Label2, Label3.
+Do not put any other text in your answer, only one or more of the provided labels with nothing before or after.
+If the text cannot be classified into any of the provided labels, answer `==NONE==`.
+
+Here is the text that needs classification
+
+
+Text:
+'''
+You look gorgeous!
+'''
+
+Backend response for doc: You look gorgeous!
+COMPLIMENT
+```
+
+`print(doc.cats)` to standard output should look like:
+
+```
+{'COMPLIMENT': 1.0, 'INSULT': 0.0}
+```
+
 ## 📓 API
 
-Each `llm` component is defined by two main settings:
+`spacy-llm` exposes a `llm` factory that accepts the following configuration options:
+
+| Argument  | Type                                        | Description                                                                         |
+| --------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
+| `task`    | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
+| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
+| `cache`   | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
+| `save_io` | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`                  |
+
+An `llm` component is defined by two main settings:
 
 - A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
 - A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
 
-Moreover, the component also implements [**caching**](#cache) functionality to avoid running
+Moreover, `spacy-llm` exposes a customizable [**caching**](#cache) functionality to avoid running
 the same document through an LLM service (be it local or through a REST API) more than once.
 
+Finally, you can choose to save a stringified version of LLM prompts/responses
+within the `Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
+`Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM component
+within the spaCy pipeline. Each entry is itself a dictionary, with two keys:
+`prompt` and `response`.
+
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
@@ -371,15 +450,14 @@
 | `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
 | `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
-
 The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured by the following parameters:
 
 - The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
   want to mark it every time it occurs in the document.
 - The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
 - The `alignment_mode` argument is used to match entities as returned by the LLM to the tokens from the original `Doc` - specifically it's used as argument
@@ -595,14 +673,79 @@
 @llm_tasks = "spacy.REL.v1"
 labels = ["LivesIn", "Visits"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "rel_examples.jsonl"
 ```
 
+#### spacy.Lemma.v1
+
+The `Lemma.v1` task lemmatizes the provided text and updates the `lemma_` attribute in the doc's tokens accordingly.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Lemma.v1"
+examples = null
+```
+
+| Argument                  | Type                                    | Default                                                   | Description                                                                                                                                           |
+| ------------------------- | --------------------------------------- |-----------------------------------------------------------| ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `template`                | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                    | Optional function that generates examples for few-shot learning.                                                                                      |
+
+`Lemma.v1` prompts the LLM to lemmatize the passed text and return the lemmatized version as a list of tokens and their
+corresponding lemma. E. g. the text 
+`I'm buying ice cream for my friends` should invoke the response
+```
+I: I
+'m: be
+buying: buy
+ice: ice
+cream: cream
+for: for
+my: my
+friends: friend
+.: .
+```
+
+If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized 
+by spaCy, no lemmas are stored in the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is updated with
+the lemma suggested by the LLM.
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```yaml
+- text: I'm buying ice cream.
+  lemmas:
+    - "I": "I"
+    - "'m": "be"
+    - "buying": "buy"
+    - "ice": "ice"
+    - "cream": "cream"
+    - ".": "."
+
+- text: I've watered the plants.
+  lemmas: 
+    - "I": "I"
+    - "'ve": "have"
+    - "watered": "water"
+    - "the": "the"
+    - "plants": "plant"
+    - ".": "."
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Lemma.v1"
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "lemma_examples.yml"
+```
+
 #### spacy.NoOp.v1
 
 This task is only useful for testing - it tells the LLM to do nothing, and does not set any fields on the `docs`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
@@ -740,56 +883,145 @@
 | -------- | ------------------------------------------------------------------------------ | ------- | ------------------------------------------------------------------------------------ |
 | `api`    | `str`                                                                          |         | The name of an API supported by LangChain, e.g. "OpenAI".                            |
 | `config` | `Dict[Any, Any]`                                                               | `{}`    | Further configuration passed on to the backend.                                      |
 | `query`  | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None`  | Function that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
 
 The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for each given textual prompt.
 
-#### spacy.DollyHF.v1
+#### spacy.Dolly_HF.v1
 
 To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
 This allows you to have the setting `device=cuda:0` in your config, which ensures that the model is loaded entirely on the GPU (and fails otherwise).
 
+You can do so with
+
 ```shell
-python -m pip install "torch>=1.13.1,<2.0"
-python -m pip install "transformers>=4.28.1,<5.0"
-# Or install with spacy-llm directly
-python -m pip install "spacy-llm[transformers]"
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ```
 
 If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
 which may ultimately result in extremely slow queries.
 
 ```shell
 python -m pip install "accelerate>=0.16.0,<1.0"
 ```
 
 Example config block:
 
 ```ini
 [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1"
+@llm_backends = "spacy.Dolly_HF.v1"
 model = "databricks/dolly-v2-3b"
 ```
 
-| Argument | Type             | Default | Description                                                                                      |
-| -------- | ---------------- | ------- | ------------------------------------------------------------------------------------------------ |
-| `model`  | `str`            |         | The name of a Dolly model that is supported.                                                     |
-| `config` | `Dict[Any, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
+| Argument      | Type             | Default | Description                                                                                      |
+| ------------- | ---------------- | ------- | ------------------------------------------------------------------------------------------------ |
+| `model`       | `str`            |         | The name of a Dolly model that is supported.                                                     |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                               |
 
 Supported models (see the [Databricks models page](https://huggingface.co/databricks) on Hugging Face for details):
 
 - `"databricks/dolly-v2-3b"`
 - `"databricks/dolly-v2-7b"`
 - `"databricks/dolly-v2-12b"`
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
+#### spacy.StableLM_HF.v1
+
+To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
+
+You can do so with
+
+```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
+```
+
+If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries.
+
+```shell
+python -m pip install "accelerate>=0.16.0,<1.0"
+```
+
+Example config block:
+
+```ini
+[components.llm.backend]
+@llm_backends = "spacy.StableLM_HF.v1"
+model = "stabilityai/stablelm-tuned-alpha-7b"
+```
+
+| Argument      | Type             | Default | Description                                                                                                                  |
+| ------------- | ---------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `model`       | `str`            |         | The name of a StableLM model that is supported.                                                                              |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                                                           |
+
+Supported models (see the [Stability AI StableLM GitHub repo](https://github.com/Stability-AI/StableLM/#stablelm-alpha) for details):
+
+- `"stabilityai/stablelm-base-alpha-3b"`
+- `"stabilityai/stablelm-base-alpha-7b"`
+- `"stabilityai/stablelm-tuned-alpha-3b"`
+- `"stabilityai/stablelm-tuned-alpha-7b"`
+
+Note that Hugging Face will download this model the first time you use it - you can
+[define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
+by setting the environmental variable `HF_HOME`.
+
+#### spacy.OpenLLaMaHF.v1
+
+To use this backend, ideally you have a GPU enabled and have installed
+
+- `transformers[sentencepiece]`
+- `torch`
+- CUDA
+  in your virtual environment.
+
+You can do so with
+
+```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
+```
+
+If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries.
+
+```shell
+python -m pip install "accelerate>=0.16.0,<1.0"
+```
+
+Example config block:
+
+```ini
+[components.llm.backend]
+@llm_backends = "spacy.OpenLLaMaHF.v1"
+model = "openlm-research/open_llama_3b_350bt_preview"
+```
+
+| Argument      | Type             | Default | Description                                                                                                                  |
+| ------------- | ---------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `model`       | `str`            |         | The name of a OpenLLaMa model that is supported.                                                                             |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                                                           |
+
+Supported models (see the [OpenLM Research OpenLLaMa GitHub repo](https://github.com/openlm-research/open_llama) for details):
+
+- `"openlm-research/open_llama_3b_350bt_preview"`
+- `"openlm-research/open_llama_3b_600bt_preview"`
+- `"openlm-research/open_llama_7b_400bt_preview"`
+- `"openlm-research/open_llama_7b_700bt_preview"`
+
+Note that Hugging Face will download this model the first time you use it - you can
+[define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
+by setting the environmental variable `HF_HOME`.
+
 ### Cache
 
 Interacting with LLMs, either through an external API or a local instance, is costly.
 Since developing an NLP pipeline generally means a lot of exploration and prototyping,
 `spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run.
 
 Example config block:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.2.1 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.0 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -89,15 +89,15 @@
 Hugging Face To run this example, ensure that you have a GPU enabled, and
 `transformers`, `torch` and CUDA installed. For more background information,
 see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
 containing at least the following (or see the full example [here]
 (usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
 = "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"]
-[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" # For better
+[components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1" # For better
 performance, use databricks/dolly-v2-12b instead model = "databricks/dolly-v2-
 3b" ``` Now run: ```python from spacy_llm.util import assemble nlp = assemble
 ("config.cfg") doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that Hugging Face
 will download the `"databricks/dolly-v2-3b"` model the first time you use it.
 You can [define the cached directory](https://huggingface.co/docs/
 huggingface_hub/main/en/guides/manage-cache) by setting the environmental
@@ -128,63 +128,100 @@
 my_other_config_val: float) -> "MyTask": labels_list = split_labels(labels)
 return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
 class MyTask: def __init__(self, labels: List[str], my_other_config_val:
 float): ... def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
 ... def parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] )
 -> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
-my_other_config_val = 0.3 ``` ## ð API Each `llm` component is defined by
-two main settings: - A [**task**](#tasks), defining the prompt to send to the
-LLM as well as the functionality to parse the resulting response back into
-structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects. - A
-[**backend**](#backends) defining the model to use and how to connect to it.
-Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
-well as access to self-hosted open-source LLMs (such as using Dolly through
-Hugging Face). Moreover, the component also implements [**caching**](#cache)
+my_other_config_val = 0.3 ``` ## Logging spacy-llm has a built-in logger that
+can log the prompt sent to the LLM as well as its raw response. This logger
+uses the debug level and by default has a `logging.NullHandler()` configured.
+In order to use this logger, you can setup a simple handler like this:
+```python import logging import spacy_llm spacy_llm.logger.addHandler
+(logging.StreamHandler()) spacy_llm.logger.setLevel(logging.DEBUG) ``` > NOTE:
+Any `logging` handler will work here so you probably want to use some sort of
+rotating `FileHandler` as the generated prompts can be quite long, especially
+for tasks with few-shot examples. Then when using the pipeline you'll be able
+to view the prompt and response. E.g. with the config and code from [Example 1]
+(##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
+```python from spacy_llm.util import assemble nlp = assemble("config.cfg") doc
+= nlp("You look gorgeous!") print(doc.cats) ``` You will see `logging` output
+similar to: ``` Generated prompt for doc: You look gorgeous! You are an expert
+Text Classification system. Your task is to accept Text as input and provide a
+category for the text based on the predefined labels. Classify the text below
+to any of the following labels: COMPLIMENT, INSULT The task is non-exclusive,
+so you can provide more than one label as long as they're comma-delimited. For
+example: Label1, Label2, Label3. Do not put any other text in your answer, only
+one or more of the provided labels with nothing before or after. If the text
+cannot be classified into any of the provided labels, answer `==NONE==`. Here
+is the text that needs classification Text: ''' You look gorgeous! ''' Backend
+response for doc: You look gorgeous! COMPLIMENT ``` `print(doc.cats)` to
+standard output should look like: ``` {'COMPLIMENT': 1.0, 'INSULT': 0.0} ``` ##
+ð API `spacy-llm` exposes a `llm` factory that accepts the following
+configuration options: | Argument | Type | Description | | --------- | --------
+----------------------------------- | -----------------------------------------
+------------------------------------------ | | `task` | `Optional[LLMTask]` |
+An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks). |
+| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a
+specific LLM API. See [docs](#backends). | | `cache` | `Cache` | Cache to use
+for caching prompts and responses per doc (batch). See [docs](#cache). | |
+`save_io` | `bool` | Whether to save prompts/responses within `Doc.user_data
+["llm_io"]` | An `llm` component is defined by two main settings: - A
+[**task**](#tasks), defining the prompt to send to the LLM as well as the
+functionality to parse the resulting response back into structured fields on
+spaCy's [Doc](https://spacy.io/api/doc) objects. - A [**backend**](#backends)
+defining the model to use and how to connect to it. Note that `spacy-llm`
+supports both access to external APIs (such as OpenAI) as well as access to
+self-hosted open-source LLMs (such as using Dolly through Hugging Face).
+Moreover, `spacy-llm` exposes a customizable [**caching**](#cache)
 functionality to avoid running the same document through an LLM service (be it
-local or through a REST API) more than once. ### Tasks A _task_ defines an NLP
-problem or question, that will be sent to the LLM via a prompt. Further, the
-task defines how to parse the LLM's responses back into structured information.
-All tasks are registered in spaCy's `llm_tasks` registry. Practically speaking,
-a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`]
-(spacy_llm/ty.py). It needs to define a `generate_prompts` function and a
-`parse_responses` function. Moreover, the task may define an optional [`scorer`
-method](https://spacy.io/api/scorer#score). It should accept an iterable of
-`Example`s as input and return a score dictionary. If the `scorer` method is
-defined, `spacy-llm` will call it to evaluate the component. #### function
-`task.generate_prompts` Takes a collection of documents, and returns a
-collection of "prompts", which can be of type `Any`. Often, prompts are of type
-`str` - but this is not enforced to allow for maximum flexibility in the
-framework. | Argument | Type | Description | | ----------- | --------------- |
----------------------- | | `docs` | `Iterable[Doc]` | The input documents. | |
-**RETURNS** | `Iterable[Any]` | The generated prompts. | #### function
-`task.parse_responses` Takes a collection of LLM responses and the original
-documents, parses the responses into structured information, and sets the
-annotations on the documents. The `parse_responses` function is free to set the
-annotations in any way, including `Doc` fields like `ents`, `spans` or `cats`,
-or using custom defined fields. The `responses` are of type `Iterable[Any]`,
-though they will often be `str` objects. This depends on the return type of the
-[backend](#backends). | Argument | Type | Description | | ----------- | -------
--------- | ------------------------ | | `docs` | `Iterable[Doc]` | The input
-documents. | | `responses` | `Iterable[Any]` | The generated prompts. | |
-**RETURNS** | `Iterable[Doc]` | The annotated documents. | #### spacy.NER.v2
-The built-in NER task supports both zero-shot and few-shot prompting. This
-version also supports explicitly defining the provided labels with custom
-descriptions. ```ini [components.llm.task] @llm_tasks = "spacy.NER.v2" labels =
-["PERSON", "ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type |
-Default | Description | | ------------------------- | -------------------------
--------------- | -------------------------------------------------------- | ---
+local or through a REST API) more than once. Finally, you can choose to save a
+stringified version of LLM prompts/responses within the `Doc.user_data
+["llm_io"]` attribute by setting `save_io` to `True`. `Doc.user_data["llm_io"]`
+is a dictionary containing one entry for every LLM component within the spaCy
+pipeline. Each entry is itself a dictionary, with two keys: `prompt` and
+`response`. ### Tasks A _task_ defines an NLP problem or question, that will be
+sent to the LLM via a prompt. Further, the task defines how to parse the LLM's
+responses back into structured information. All tasks are registered in spaCy's
+`llm_tasks` registry. Practically speaking, a task should adhere to the
+`Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py). It needs to define
+a `generate_prompts` function and a `parse_responses` function. Moreover, the
+task may define an optional [`scorer` method](https://spacy.io/api/
+scorer#score). It should accept an iterable of `Example`s as input and return a
+score dictionary. If the `scorer` method is defined, `spacy-llm` will call it
+to evaluate the component. #### function `task.generate_prompts` Takes a
+collection of documents, and returns a collection of "prompts", which can be of
+type `Any`. Often, prompts are of type `str` - but this is not enforced to
+allow for maximum flexibility in the framework. | Argument | Type | Description
+| | ----------- | --------------- | ---------------------- | | `docs` |
+`Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
+generated prompts. | #### function `task.parse_responses` Takes a collection of
+LLM responses and the original documents, parses the responses into structured
+information, and sets the annotations on the documents. The `parse_responses`
+function is free to set the annotations in any way, including `Doc` fields like
+`ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
+of type `Iterable[Any]`, though they will often be `str` objects. This depends
+on the return type of the [backend](#backends). | Argument | Type | Description
+| | ----------- | --------------- | ------------------------ | | `docs` |
+`Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
+generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
+| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
+prompting. This version also supports explicitly defining the provided labels
+with custom descriptions. ```ini [components.llm.task] @llm_tasks =
+"spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"] examples = null
+``` | Argument | Type | Default | Description | | ------------------------- | -
+-------------------------------------- | --------------------------------------
+------------------ | ----------------------------------------------------------
 -------------------------------------------------------------------------------
-------------------------------------------------------------------- | |
-`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
-list of labels. | | `template` | `str` | [ner.v2.jinja](./spacy_llm/tasks/
-templates/ner.v2.jinja) | Custom prompt template to send to LLM backend.
-Default templates for each task are located in the `spacy_llm/tasks/templates`
-directory. | | `label_definitions` | `Optional[Dict[str, str]]` | `None` |
-Optional dict mapping a label to a description of that label. These
+------------ | | `labels` | `Union[List[str], str]` | | List of labels or str
+of comma-separated list of labels. | | `template` | `str` | [ner.v2.jinja](./
+spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `label_definitions` | `Optional[Dict[str, str]]` |
+`None` | Optional dict mapping a label to a description of that label. These
 descriptions are added to the prompt to help instruct the LLM on what to
 extract. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
 Optional function that generates examples for few-shot learning. | |
 `normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
 normalizes the labels as returned by the LLM. If `None`, defaults to
 `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
 Alignment mode in case the LLM returns entities that do not align with token
@@ -401,147 +438,226 @@
 "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
 "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
 the REL task relies on pre-extracted entities to make its prediction. Hence,
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
 [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
 "Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
-= "rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
-testing - it tells the LLM to do nothing, and does not set any fields on the
-`docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
-Backends A _backend_ defines which LLM model to query, and how to query it. It
-can be a simple function taking a collection of prompts (consistent with the
-output type of `task.generate_prompts()`) and returning a collection of
-responses (consistent with the expected input of `parse_responses`). Generally
-speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
-but specific implementations can have other signatures, like `Callable[
-[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
-`llm_backends`. If no backend is specified, the repo currently connects to the
-[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
-accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
-third-party libraries in addition to a native REST backend and which should > I
-choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
-prompt management, integration of many different LLM > APIs, and other related
-features such as conversational memory or agents. `spacy-llm` on the other hand
-emphasizes > features we consider useful in the context of NLP pipelines
-utilizing LLMs to process documents (mostly) independent > from each other. It
-makes sense that the feature set of such third-party libraries and `spacy-llm`
-is not identical - > and users might want to take advantage of features not
-available in `spacy-llm`. > > The advantage of offering our own REST backend is
-that we can ensure a larger degree of stability of robustness, as > we can
-guarantee backwards-compatibility and more smoothly integrated error handling.
-> > Ultimately we recommend trying to implement your use case using the REST
-backend first (which is configured as the > default backend). If however there
-are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
-> backend of a third-party library - and easy to customize the prompting
-mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
-to get an API key from openai.com, and ensure that the keys are set as
-environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
-OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
-`requests` and a simple retry mechanism to access an API. ```ini
-[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
-= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
-Default | Description | | ----------- | ---------------- | ------- | ----------
+= "rel_examples.jsonl" ``` #### spacy.Lemma.v1 The `Lemma.v1` task lemmatizes
+the provided text and updates the `lemma_` attribute in the doc's tokens
+accordingly. ```ini [components.llm.task] @llm_tasks = "spacy.Lemma.v1"
+examples = null ``` | Argument | Type | Default | Description | | -------------
+------------ | --------------------------------------- |-----------------------
+------------------------------------| -----------------------------------------
 -------------------------------------------------------------------------------
---------------------------- | | `api` | `str` | | The name of a supported API.
-In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
-| Further configuration passed on to the backend. | | `strict` | `bool` |
-`True` | If `True`, raises an error if the LLM API returns a malformed
-response. Otherwise, return the error responses as is. | | `max_tries` | `int`
-| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
-Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
-following settings can be defined in the `config` dictionary: - `model`: one of
-the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
-`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
-babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
-`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
-For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
-completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
-srush/MiniChain) for the API retrieval part, make sure you have installed it
-first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
-spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
-MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
-blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
-api = "OpenAI" [components.llm.backend.query] @llm_queries =
-"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
---- | -------------------------------------------------------------------------
--------- | ------- | ----------------------------------------------------------
-------------------------- | | `api` | `str` | | The name of an API supported by
-MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
-configuration passed on to the backend. | | `query` | `Optional[Callable[
-["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
-Function that executes the prompts. If `None`, defaults to
-`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
-executes the prompts by running `model(text).run()` for each given textual
-prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
-hwchase17/langchain) for the API retrieval part, make sure you have installed
-it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
-with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
-that LangChain currently only supports Python 3.9 and beyond. Example config
-block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
-= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
-{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
-- | ---------------------------------------------------------------------------
---- | ------- | ---------------------------------------------------------------
---------------------- | | `api` | `str` | | The name of an API supported by
-LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
-configuration passed on to the backend. | | `query` | `Optional[Callable[
-["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
-that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
-The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
-`model(text)` for each given textual prompt. #### spacy.DollyHF.v1 To use this
+----------------------------- | | `template` | `str` | [lemma.jinja](./
+spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
+| `None` | Optional function that generates examples for few-shot learning. |
+`Lemma.v1` prompts the LLM to lemmatize the passed text and return the
+lemmatized version as a list of tokens and their corresponding lemma. E. g. the
+text `I'm buying ice cream for my friends` should invoke the response ``` I: I
+'m: be buying: buy ice: ice cream: cream for: for my: my friends: friend .: .
+``` If for any given text/doc instance the number of lemmas returned by the LLM
+doesn't match the number of tokens recognized by spaCy, no lemmas are stored in
+the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is
+updated with the lemma suggested by the LLM. To perform few-shot learning, you
+can write down a few examples in a separate file, and provide these to be
+injected into the prompt to the LLM. The default reader
+`spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+```yaml - text: I'm buying ice cream. lemmas: - "I": "I" - "'m": "be" -
+"buying": "buy" - "ice": "ice" - "cream": "cream" - ".": "." - text: I've
+watered the plants. lemmas: - "I": "I" - "'ve": "have" - "watered": "water" -
+"the": "the" - "plants": "plant" - ".": "." ``` ```ini [components.llm.task]
+@llm_tasks = "spacy.Lemma.v1" [components.llm.task.examples] @misc =
+"spacy.FewShotReader.v1" path = "lemma_examples.yml" ``` #### spacy.NoOp.v1
+This task is only useful for testing - it tells the LLM to do nothing, and does
+not set any fields on the `docs`. ```ini [components.llm.task] @llm_tasks =
+"spacy.NoOp.v1" ``` ### Backends A _backend_ defines which LLM model to query,
+and how to query it. It can be a simple function taking a collection of prompts
+(consistent with the output type of `task.generate_prompts()`) and returning a
+collection of responses (consistent with the expected input of
+`parse_responses`). Generally speaking, it's a function of type `Callable[
+[Iterable[Any]], Iterable[Any]]`, but specific implementations can have other
+signatures, like `Callable[[Iterable[str]], Iterable[str]]`. All built-in
+backends are registered in `llm_backends`. If no backend is specified, the repo
+currently connects to the [`OpenAI` API](#openai) by default, using the built-
+in REST protocol, and accesses the `"gpt-3.5-turbo"` model. > :question: _Why
+are there backends for third-party libraries in addition to a native REST
+backend and which should > I choose?_ > > Third-party libraries like
+`langchain` or `minichain` focus on prompt management, integration of many
+different LLM > APIs, and other related features such as conversational memory
+or agents. `spacy-llm` on the other hand emphasizes > features we consider
+useful in the context of NLP pipelines utilizing LLMs to process documents
+(mostly) independent > from each other. It makes sense that the feature set of
+such third-party libraries and `spacy-llm` is not identical - > and users might
+want to take advantage of features not available in `spacy-llm`. > > The
+advantage of offering our own REST backend is that we can ensure a larger
+degree of stability of robustness, as > we can guarantee backwards-
+compatibility and more smoothly integrated error handling. > > Ultimately we
+recommend trying to implement your use case using the REST backend first (which
+is configured as the > default backend). If however there are features or APIs
+not covered by `spacy-llm`, it's trivial to switch to the > backend of a third-
+party library - and easy to customize the prompting mechanism, if so required.
+#### OpenAI When the backend uses OpenAI, you have to get an API key from
+openai.com, and ensure that the keys are set as environmental variables:
+```shell export OPENAI_API_KEY="sk-..." export OPENAI_API_ORG="org-..." ```
+#### spacy.REST.v1 This default backend uses `requests` and a simple retry
+mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
+"spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-turbo",
+"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
+-- | ---------------- | ------- | ---------------------------------------------
+----------------------------------------------------------------------- | |
+`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
+supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
+passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
+error if the LLM API returns a malformed response. Otherwise, return the error
+responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
+request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
+When `api` is set to `OpenAI`, the following settings can be defined in the
+`config` dictionary: - `model`: one of the following list of supported models:
+- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
+turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
+- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
+`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
+api.openai.com/v1/completions`. For models requiring the chat endpoint, use
+`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
+[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
+make sure you have installed it first: ```shell python -m pip install
+"minichain>=0.3,<0.4" # Or install with spacy-llm directly python -m pip
+install "spacy-llm[minichain]" ``` Note that MiniChain currently only supports
+Python 3.8, 3.9 and 3.10. Example config blocks: ```ini
+[components.llm.backend] @llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
+[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
+Argument | Type | Default | Description | | -------- | ------------------------
+--------------------------------------------------------- | ------- | ---------
+-------------------------------------------------------------------------- | |
+`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
+`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
+backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
+Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
+If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
+(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
+for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
+(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
+you have installed it first: ```shell python -m pip install
+"langchain>=0.0.144,<0.1" # Or install with spacy-llm directly python -m pip
+install "spacy-llm[langchain]" ``` Note that LangChain currently only supports
+Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
+@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
+"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
+Default | Description | | -------- | ------------------------------------------
+------------------------------------ | ------- | ------------------------------
+------------------------------------------------------ | | `api` | `str` | |
+The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
+[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
+`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
+Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
+defaults to `spacy.CallLangChain.v1`. | The default `query`
+(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
+each given textual prompt. #### spacy.Dolly_HF.v1 To use this backend, ideally
+you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
+your virtual environment. This allows you to have the setting `device=cuda:0`
+in your config, which ensures that the model is loaded entirely on the GPU (and
+fails otherwise). You can do so with ```shell python -m pip install "spacy-llm
+[transformers]" "transformers[sentencepiece]" ``` If you don't have access to a
+GPU, you can install `accelerate` and set`device_map=auto` instead, but be
+aware that this may result in some layers getting distributed to the CPU or
+even the hard drive, which may ultimately result in extremely slow queries.
+```shell python -m pip install "accelerate>=0.16.0,<1.0" ``` Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1"
+model = "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description
+| | ------------- | ---------------- | ------- | ------------------------------
+------------------------------------------------------------------ | | `model`
+| `str` | | The name of a Dolly model that is supported. | | `config_init` |
+`Dict[str, Any]` | `{}` | Further configuration passed on to the construction
+of the model with `transformers.pipeline()`. | | `config_run` | `Dict[str,
+Any]` | `{}` | Further configuration used during model inference. | Supported
+models (see the [Databricks models page](https://huggingface.co/databricks) on
+Hugging Face for details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-
+v2-7b"` - `"databricks/dolly-v2-12b"` Note that Hugging Face will download this
+model the first time you use it - you can [define the cached directory](https:/
+/huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting
+the environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
 backend, ideally you have a GPU enabled and have installed `transformers`,
-`torch` and CUDA in your virtual environment. This allows you to have the
-setting `device=cuda:0` in your config, which ensures that the model is loaded
-entirely on the GPU (and fails otherwise). ```shell python -m pip install
-"torch>=1.13.1,<2.0" python -m pip install "transformers>=4.28.1,<5.0" # Or
-install with spacy-llm directly python -m pip install "spacy-llm[transformers]"
+`torch` and CUDA in your virtual environment. You can do so with ```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ``` If you don't have access to a GPU, you can install `accelerate` and
 set`device_map=auto` instead, but be aware that this may result in some layers
 getting distributed to the CPU or even the hard drive, which may ultimately
 result in extremely slow queries. ```shell python -m pip install
 "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
-[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" model =
-"databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
----- | ---------------- | ------- | -------------------------------------------
------------------------------------------------------ | | `model` | `str` | |
-The name of a Dolly model that is supported. | | `config` | `Dict[Any, Any]` |
-`{}` | Further configuration passed on to the construction of the model with
-`transformers.pipeline()`. | Supported models (see the [Databricks models page]
-(https://huggingface.co/databricks) on Hugging Face for details): -
-`"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` - `"databricks/dolly-
-v2-12b"` Note that Hugging Face will download this model the first time you use
-it - you can [define the cached directory](https://huggingface.co/docs/
+[components.llm.backend] @llm_backends = "spacy.StableLM_HF.v1" model =
+"stabilityai/stablelm-tuned-alpha-7b" ``` | Argument | Type | Default |
+Description | | ------------- | ---------------- | ------- | ------------------
+-------------------------------------------------------------------------------
+--------------------------- | | `model` | `str` | | The name of a StableLM
+model that is supported. | | `config_init` | `Dict[str, Any]` | `{}` | Further
+configuration passed on to the construction of the model with
+`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
+[str, Any]` | `{}` | Further configuration used during model inference. |
+Supported models (see the [Stability AI StableLM GitHub repo](https://
+github.com/Stability-AI/StableLM/#stablelm-alpha) for details): -
+`"stabilityai/stablelm-base-alpha-3b"` - `"stabilityai/stablelm-base-alpha-7b"`
+- `"stabilityai/stablelm-tuned-alpha-3b"` - `"stabilityai/stablelm-tuned-alpha-
+7b"` Note that Hugging Face will download this model the first time you use it
+- you can [define the cached directory](https://huggingface.co/docs/
 huggingface_hub/main/en/guides/manage-cache) by setting the environmental
-variable `HF_HOME`. ### Cache Interacting with LLMs, either through an external
-API or a local instance, is costly. Since developing an NLP pipeline generally
-means a lot of exploration and prototyping, `spacy-llm` implements a built-in
-cache to avoid reprocessing the same documents at each run. Example config
-block: ```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1", path =
-"path/to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
-Default | Description | | -------------------- | ---------------------------- |
-------- | ---------------------------------------------------- | | `path` |
-`Optional[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching
-is performed. | | `batch_size` | `int` | 64 | Number of docs in one batch
-(file). | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
-in memory. | Note that since the cache is generated by a registered function,
-you can also provide your own registered function returning your own cache
-implementation. If you wish to do so, ensure that your cache object adheres to
-the `Protocol` defined in `spacy_llm.ty.Cache`. ### Various functions ####
-spacy.FewShotReader.v1 This function is registered in spaCy's `misc` registry,
-and reads in examples from a `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses
-[`srsly`](https://github.com/explosion/srsly) to read in these files and parses
-them depending on the file extension. ```ini [components.llm.task.examples]
-@misc = "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument |
-Type | Description | | -------- | ------------------ | ------------------------
--------------------------------------------------- | | `path` | `Union[str,
-Path]` | Path to an examples file with suffix `.yml`, `.yaml`, `.json` or
-`.jsonl`. | #### spacy.FileReader.v1 This function is registered in spaCy's
-`misc` registry, and reads a file provided to the `path` to return a `str`
+variable `HF_HOME`. #### spacy.OpenLLaMaHF.v1 To use this backend, ideally you
+have a GPU enabled and have installed - `transformers[sentencepiece]` - `torch`
+- CUDA in your virtual environment. You can do so with ```shell python -m pip
+install "spacy-llm[transformers]" "transformers[sentencepiece]" ``` If you
+don't have access to a GPU, you can install `accelerate` and
+set`device_map=auto` instead, but be aware that this may result in some layers
+getting distributed to the CPU or even the hard drive, which may ultimately
+result in extremely slow queries. ```shell python -m pip install
+"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.backend] @llm_backends = "spacy.OpenLLaMaHF.v1" model =
+"openlm-research/open_llama_3b_350bt_preview" ``` | Argument | Type | Default |
+Description | | ------------- | ---------------- | ------- | ------------------
+-------------------------------------------------------------------------------
+--------------------------- | | `model` | `str` | | The name of a OpenLLaMa
+model that is supported. | | `config_init` | `Dict[str, Any]` | `{}` | Further
+configuration passed on to the construction of the model with
+`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
+[str, Any]` | `{}` | Further configuration used during model inference. |
+Supported models (see the [OpenLM Research OpenLLaMa GitHub repo](https://
+github.com/openlm-research/open_llama) for details): - `"openlm-research/
+open_llama_3b_350bt_preview"` - `"openlm-research/open_llama_3b_600bt_preview"`
+- `"openlm-research/open_llama_7b_400bt_preview"` - `"openlm-research/
+open_llama_7b_700bt_preview"` Note that Hugging Face will download this model
+the first time you use it - you can [define the cached directory](https://
+huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
+environmental variable `HF_HOME`. ### Cache Interacting with LLMs, either
+through an external API or a local instance, is costly. Since developing an NLP
+pipeline generally means a lot of exploration and prototyping, `spacy-llm`
+implements a built-in cache to avoid reprocessing the same documents at each
+run. Example config block: ```ini [components.llm.cache] @llm_misc =
+"spacy.BatchCache.v1", path = "path/to/cache" batch_size = 64
+max_batches_in_mem = 4 ``` | Argument | Type | Default | Description | | ------
+-------------- | ---------------------------- | ------- | ---------------------
+------------------------------- | | `path` | `Optional[Union[str, Path]]` |
+`None` | Cache directory. If `None`, no caching is performed. | | `batch_size`
+| `int` | 64 | Number of docs in one batch (file). | | `max_batches_in_mem` |
+`int` | 4 | Max. number of batches to hold in memory. | Note that since the
+cache is generated by a registered function, you can also provide your own
+registered function returning your own cache implementation. If you wish to do
+so, ensure that your cache object adheres to the `Protocol` defined in
+`spacy_llm.ty.Cache`. ### Various functions #### spacy.FewShotReader.v1 This
+function is registered in spaCy's `misc` registry, and reads in examples from a
+`.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
+github.com/explosion/srsly) to read in these files and parses them depending on
+the file extension. ```ini [components.llm.task.examples] @misc =
+"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument | Type |
+Description | | -------- | ------------------ | -------------------------------
+------------------------------------------- | | `path` | `Union[str, Path]` |
+Path to an examples file with suffix `.yml`, `.yaml`, `.json` or `.jsonl`. |
+#### spacy.FileReader.v1 This function is registered in spaCy's `misc`
+registry, and reads a file provided to the `path` to return a `str`
 representation of its contents. This function is typically used to read [Jinja]
 (https://jinja.palletsprojects.com/en/3.1.x/) files containing the prompt
 template. ```ini [components.llm.task.template] @misc = "spacy.FileReader.v1"
 path = "ner_template.jinja2" ``` | Argument | Type | Description | | -------- |
 ------------------ | ---------------------------- | | `path` | `Union[str,
 Path]` | Path to the file to be read. | #### Normalizer functions These
 functions provide simple normalizations for string comparisons, e.g. between a
```

### Comparing `spacy-llm-0.2.1/README.md` & `spacy-llm-0.3.0/spacy_llm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: spacy-llm
+Version: 0.3.0
+Summary: Integrating LLMs into structured NLP pipelines
+Author: Explosion
+Author-email: contact@explosion.ai
+License: MIT
+Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
+Project-URL: Source, https://github.com/explosion/spacy-llm
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: minichain
+Provides-Extra: langchain
+Provides-Extra: transformers
+License-File: LICENSE
+
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
@@ -102,15 +134,15 @@
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
 labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
 [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1"
+@llm_backends = "spacy.Dolly_HF.v1"
 # For better performance, use databricks/dolly-v2-12b instead
 model = "databricks/dolly-v2-3b"
 ```
 
 Now run:
 
 ```python
@@ -198,26 +230,105 @@
 # config.cfg (excerpt)
 [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1"
 labels = LABEL1,LABEL2,LABEL3
 my_other_config_val = 0.3
 ```
 
+## Logging
+
+spacy-llm has a built-in logger that can log the prompt sent to the LLM as well as its raw response. This logger uses the debug level and by default has a `logging.NullHandler()` configured.
+
+In order to use this logger, you can setup a simple handler like this:
+
+```python
+import logging
+import spacy_llm
+
+
+spacy_llm.logger.addHandler(logging.StreamHandler())
+spacy_llm.logger.setLevel(logging.DEBUG)
+```
+
+> NOTE: Any `logging` handler will work here so you probably want to use some sort of rotating `FileHandler` as the generated prompts can be quite long, especially for tasks with few-shot examples.
+
+
+Then when using the pipeline you'll be able to view the prompt and response.
+
+E.g. with the config and code from [Example 1](##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
+
+
+```python
+from spacy_llm.util import assemble
+
+
+nlp = assemble("config.cfg")
+doc = nlp("You look gorgeous!")
+print(doc.cats)
+```
+
+You will see `logging` output similar to:
+
+```
+Generated prompt for doc: You look gorgeous!
+
+You are an expert Text Classification system. Your task is to accept Text as input
+and provide a category for the text based on the predefined labels.
+
+Classify the text below to any of the following labels: COMPLIMENT, INSULT
+The task is non-exclusive, so you can provide more than one label as long as
+they're comma-delimited. For example: Label1, Label2, Label3.
+Do not put any other text in your answer, only one or more of the provided labels with nothing before or after.
+If the text cannot be classified into any of the provided labels, answer `==NONE==`.
+
+Here is the text that needs classification
+
+
+Text:
+'''
+You look gorgeous!
+'''
+
+Backend response for doc: You look gorgeous!
+COMPLIMENT
+```
+
+`print(doc.cats)` to standard output should look like:
+
+```
+{'COMPLIMENT': 1.0, 'INSULT': 0.0}
+```
+
 ## 📓 API
 
-Each `llm` component is defined by two main settings:
+`spacy-llm` exposes a `llm` factory that accepts the following configuration options:
+
+| Argument  | Type                                        | Description                                                                         |
+| --------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
+| `task`    | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
+| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
+| `cache`   | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
+| `save_io` | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`                  |
+
+An `llm` component is defined by two main settings:
 
 - A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
 - A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
 
-Moreover, the component also implements [**caching**](#cache) functionality to avoid running
+Moreover, `spacy-llm` exposes a customizable [**caching**](#cache) functionality to avoid running
 the same document through an LLM service (be it local or through a REST API) more than once.
 
+Finally, you can choose to save a stringified version of LLM prompts/responses
+within the `Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
+`Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM component
+within the spaCy pipeline. Each entry is itself a dictionary, with two keys:
+`prompt` and `response`.
+
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
@@ -339,15 +450,14 @@
 | `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
 | `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
-
 The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured by the following parameters:
 
 - The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
   want to mark it every time it occurs in the document.
 - The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
 - The `alignment_mode` argument is used to match entities as returned by the LLM to the tokens from the original `Doc` - specifically it's used as argument
@@ -563,14 +673,79 @@
 @llm_tasks = "spacy.REL.v1"
 labels = ["LivesIn", "Visits"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "rel_examples.jsonl"
 ```
 
+#### spacy.Lemma.v1
+
+The `Lemma.v1` task lemmatizes the provided text and updates the `lemma_` attribute in the doc's tokens accordingly.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Lemma.v1"
+examples = null
+```
+
+| Argument                  | Type                                    | Default                                                   | Description                                                                                                                                           |
+| ------------------------- | --------------------------------------- |-----------------------------------------------------------| ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `template`                | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                    | Optional function that generates examples for few-shot learning.                                                                                      |
+
+`Lemma.v1` prompts the LLM to lemmatize the passed text and return the lemmatized version as a list of tokens and their
+corresponding lemma. E. g. the text 
+`I'm buying ice cream for my friends` should invoke the response
+```
+I: I
+'m: be
+buying: buy
+ice: ice
+cream: cream
+for: for
+my: my
+friends: friend
+.: .
+```
+
+If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized 
+by spaCy, no lemmas are stored in the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is updated with
+the lemma suggested by the LLM.
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```yaml
+- text: I'm buying ice cream.
+  lemmas:
+    - "I": "I"
+    - "'m": "be"
+    - "buying": "buy"
+    - "ice": "ice"
+    - "cream": "cream"
+    - ".": "."
+
+- text: I've watered the plants.
+  lemmas: 
+    - "I": "I"
+    - "'ve": "have"
+    - "watered": "water"
+    - "the": "the"
+    - "plants": "plant"
+    - ".": "."
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Lemma.v1"
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "lemma_examples.yml"
+```
+
 #### spacy.NoOp.v1
 
 This task is only useful for testing - it tells the LLM to do nothing, and does not set any fields on the `docs`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
@@ -708,56 +883,145 @@
 | -------- | ------------------------------------------------------------------------------ | ------- | ------------------------------------------------------------------------------------ |
 | `api`    | `str`                                                                          |         | The name of an API supported by LangChain, e.g. "OpenAI".                            |
 | `config` | `Dict[Any, Any]`                                                               | `{}`    | Further configuration passed on to the backend.                                      |
 | `query`  | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None`  | Function that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
 
 The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for each given textual prompt.
 
-#### spacy.DollyHF.v1
+#### spacy.Dolly_HF.v1
 
 To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
 This allows you to have the setting `device=cuda:0` in your config, which ensures that the model is loaded entirely on the GPU (and fails otherwise).
 
+You can do so with
+
 ```shell
-python -m pip install "torch>=1.13.1,<2.0"
-python -m pip install "transformers>=4.28.1,<5.0"
-# Or install with spacy-llm directly
-python -m pip install "spacy-llm[transformers]"
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ```
 
 If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
 which may ultimately result in extremely slow queries.
 
 ```shell
 python -m pip install "accelerate>=0.16.0,<1.0"
 ```
 
 Example config block:
 
 ```ini
 [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1"
+@llm_backends = "spacy.Dolly_HF.v1"
 model = "databricks/dolly-v2-3b"
 ```
 
-| Argument | Type             | Default | Description                                                                                      |
-| -------- | ---------------- | ------- | ------------------------------------------------------------------------------------------------ |
-| `model`  | `str`            |         | The name of a Dolly model that is supported.                                                     |
-| `config` | `Dict[Any, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
+| Argument      | Type             | Default | Description                                                                                      |
+| ------------- | ---------------- | ------- | ------------------------------------------------------------------------------------------------ |
+| `model`       | `str`            |         | The name of a Dolly model that is supported.                                                     |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                               |
 
 Supported models (see the [Databricks models page](https://huggingface.co/databricks) on Hugging Face for details):
 
 - `"databricks/dolly-v2-3b"`
 - `"databricks/dolly-v2-7b"`
 - `"databricks/dolly-v2-12b"`
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
+#### spacy.StableLM_HF.v1
+
+To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
+
+You can do so with
+
+```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
+```
+
+If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries.
+
+```shell
+python -m pip install "accelerate>=0.16.0,<1.0"
+```
+
+Example config block:
+
+```ini
+[components.llm.backend]
+@llm_backends = "spacy.StableLM_HF.v1"
+model = "stabilityai/stablelm-tuned-alpha-7b"
+```
+
+| Argument      | Type             | Default | Description                                                                                                                  |
+| ------------- | ---------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `model`       | `str`            |         | The name of a StableLM model that is supported.                                                                              |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                                                           |
+
+Supported models (see the [Stability AI StableLM GitHub repo](https://github.com/Stability-AI/StableLM/#stablelm-alpha) for details):
+
+- `"stabilityai/stablelm-base-alpha-3b"`
+- `"stabilityai/stablelm-base-alpha-7b"`
+- `"stabilityai/stablelm-tuned-alpha-3b"`
+- `"stabilityai/stablelm-tuned-alpha-7b"`
+
+Note that Hugging Face will download this model the first time you use it - you can
+[define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
+by setting the environmental variable `HF_HOME`.
+
+#### spacy.OpenLLaMaHF.v1
+
+To use this backend, ideally you have a GPU enabled and have installed
+
+- `transformers[sentencepiece]`
+- `torch`
+- CUDA
+  in your virtual environment.
+
+You can do so with
+
+```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
+```
+
+If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries.
+
+```shell
+python -m pip install "accelerate>=0.16.0,<1.0"
+```
+
+Example config block:
+
+```ini
+[components.llm.backend]
+@llm_backends = "spacy.OpenLLaMaHF.v1"
+model = "openlm-research/open_llama_3b_350bt_preview"
+```
+
+| Argument      | Type             | Default | Description                                                                                                                  |
+| ------------- | ---------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `model`       | `str`            |         | The name of a OpenLLaMa model that is supported.                                                                             |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                                                           |
+
+Supported models (see the [OpenLM Research OpenLLaMa GitHub repo](https://github.com/openlm-research/open_llama) for details):
+
+- `"openlm-research/open_llama_3b_350bt_preview"`
+- `"openlm-research/open_llama_3b_600bt_preview"`
+- `"openlm-research/open_llama_7b_400bt_preview"`
+- `"openlm-research/open_llama_7b_700bt_preview"`
+
+Note that Hugging Face will download this model the first time you use it - you can
+[define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
+by setting the environmental variable `HF_HOME`.
+
 ### Cache
 
 Interacting with LLMs, either through an external API or a local instance, is costly.
 Since developing an NLP pipeline generally means a lot of exploration and prototyping,
 `spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run.
 
 Example config block:
```

#### html2text {}

```diff
@@ -1,12 +1,29 @@
-[https://explosion.ai/assets/img/logo.svg] # spacy-llm: Integrating LLMs into
-structured NLP pipelines [![GitHub Workflow Status](https://img.shields.io/
-github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)]
-(https://github.com/explosion/spacy-llm/actions/workflows/test.yml) [![pypi
-Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.3.0 Summary: Integrating LLMs
+into structured NLP pipelines Author: Explosion Author-email:
+contact@explosion.ai License: MIT Project-URL: Release notes, https://
+github.com/explosion/spacy-llm/releases Project-URL: Source, https://
+github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
+Content-Type: text/markdown Provides-Extra: minichain Provides-Extra: langchain
+Provides-Extra: transformers License-File: LICENSE [https://explosion.ai/
+assets/img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP
+pipelines [![GitHub Workflow Status](https://img.shields.io/github/actions/
+workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/
+explosion/spacy-llm/actions/workflows/test.yml) [![pypi Version](https://
+img.shields.io/pypi/v/spacy-llm.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg?style=flat-square)](https://github.com/ambv/black) This package
 integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
 featuring a modular system for **fast prototyping** and **prompting**, and
 turning unstructured responses into **robust outputs** for various NLP tasks,
 **no training data** required. - Serializable `llm` **component** to integrate
@@ -72,15 +89,15 @@
 Hugging Face To run this example, ensure that you have a GPU enabled, and
 `transformers`, `torch` and CUDA installed. For more background information,
 see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
 containing at least the following (or see the full example [here]
 (usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
 = "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"]
-[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" # For better
+[components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1" # For better
 performance, use databricks/dolly-v2-12b instead model = "databricks/dolly-v2-
 3b" ``` Now run: ```python from spacy_llm.util import assemble nlp = assemble
 ("config.cfg") doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that Hugging Face
 will download the `"databricks/dolly-v2-3b"` model the first time you use it.
 You can [define the cached directory](https://huggingface.co/docs/
 huggingface_hub/main/en/guides/manage-cache) by setting the environmental
@@ -111,63 +128,100 @@
 my_other_config_val: float) -> "MyTask": labels_list = split_labels(labels)
 return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
 class MyTask: def __init__(self, labels: List[str], my_other_config_val:
 float): ... def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
 ... def parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] )
 -> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
-my_other_config_val = 0.3 ``` ## ð API Each `llm` component is defined by
-two main settings: - A [**task**](#tasks), defining the prompt to send to the
-LLM as well as the functionality to parse the resulting response back into
-structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects. - A
-[**backend**](#backends) defining the model to use and how to connect to it.
-Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
-well as access to self-hosted open-source LLMs (such as using Dolly through
-Hugging Face). Moreover, the component also implements [**caching**](#cache)
+my_other_config_val = 0.3 ``` ## Logging spacy-llm has a built-in logger that
+can log the prompt sent to the LLM as well as its raw response. This logger
+uses the debug level and by default has a `logging.NullHandler()` configured.
+In order to use this logger, you can setup a simple handler like this:
+```python import logging import spacy_llm spacy_llm.logger.addHandler
+(logging.StreamHandler()) spacy_llm.logger.setLevel(logging.DEBUG) ``` > NOTE:
+Any `logging` handler will work here so you probably want to use some sort of
+rotating `FileHandler` as the generated prompts can be quite long, especially
+for tasks with few-shot examples. Then when using the pipeline you'll be able
+to view the prompt and response. E.g. with the config and code from [Example 1]
+(##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
+```python from spacy_llm.util import assemble nlp = assemble("config.cfg") doc
+= nlp("You look gorgeous!") print(doc.cats) ``` You will see `logging` output
+similar to: ``` Generated prompt for doc: You look gorgeous! You are an expert
+Text Classification system. Your task is to accept Text as input and provide a
+category for the text based on the predefined labels. Classify the text below
+to any of the following labels: COMPLIMENT, INSULT The task is non-exclusive,
+so you can provide more than one label as long as they're comma-delimited. For
+example: Label1, Label2, Label3. Do not put any other text in your answer, only
+one or more of the provided labels with nothing before or after. If the text
+cannot be classified into any of the provided labels, answer `==NONE==`. Here
+is the text that needs classification Text: ''' You look gorgeous! ''' Backend
+response for doc: You look gorgeous! COMPLIMENT ``` `print(doc.cats)` to
+standard output should look like: ``` {'COMPLIMENT': 1.0, 'INSULT': 0.0} ``` ##
+ð API `spacy-llm` exposes a `llm` factory that accepts the following
+configuration options: | Argument | Type | Description | | --------- | --------
+----------------------------------- | -----------------------------------------
+------------------------------------------ | | `task` | `Optional[LLMTask]` |
+An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks). |
+| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a
+specific LLM API. See [docs](#backends). | | `cache` | `Cache` | Cache to use
+for caching prompts and responses per doc (batch). See [docs](#cache). | |
+`save_io` | `bool` | Whether to save prompts/responses within `Doc.user_data
+["llm_io"]` | An `llm` component is defined by two main settings: - A
+[**task**](#tasks), defining the prompt to send to the LLM as well as the
+functionality to parse the resulting response back into structured fields on
+spaCy's [Doc](https://spacy.io/api/doc) objects. - A [**backend**](#backends)
+defining the model to use and how to connect to it. Note that `spacy-llm`
+supports both access to external APIs (such as OpenAI) as well as access to
+self-hosted open-source LLMs (such as using Dolly through Hugging Face).
+Moreover, `spacy-llm` exposes a customizable [**caching**](#cache)
 functionality to avoid running the same document through an LLM service (be it
-local or through a REST API) more than once. ### Tasks A _task_ defines an NLP
-problem or question, that will be sent to the LLM via a prompt. Further, the
-task defines how to parse the LLM's responses back into structured information.
-All tasks are registered in spaCy's `llm_tasks` registry. Practically speaking,
-a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`]
-(spacy_llm/ty.py). It needs to define a `generate_prompts` function and a
-`parse_responses` function. Moreover, the task may define an optional [`scorer`
-method](https://spacy.io/api/scorer#score). It should accept an iterable of
-`Example`s as input and return a score dictionary. If the `scorer` method is
-defined, `spacy-llm` will call it to evaluate the component. #### function
-`task.generate_prompts` Takes a collection of documents, and returns a
-collection of "prompts", which can be of type `Any`. Often, prompts are of type
-`str` - but this is not enforced to allow for maximum flexibility in the
-framework. | Argument | Type | Description | | ----------- | --------------- |
----------------------- | | `docs` | `Iterable[Doc]` | The input documents. | |
-**RETURNS** | `Iterable[Any]` | The generated prompts. | #### function
-`task.parse_responses` Takes a collection of LLM responses and the original
-documents, parses the responses into structured information, and sets the
-annotations on the documents. The `parse_responses` function is free to set the
-annotations in any way, including `Doc` fields like `ents`, `spans` or `cats`,
-or using custom defined fields. The `responses` are of type `Iterable[Any]`,
-though they will often be `str` objects. This depends on the return type of the
-[backend](#backends). | Argument | Type | Description | | ----------- | -------
--------- | ------------------------ | | `docs` | `Iterable[Doc]` | The input
-documents. | | `responses` | `Iterable[Any]` | The generated prompts. | |
-**RETURNS** | `Iterable[Doc]` | The annotated documents. | #### spacy.NER.v2
-The built-in NER task supports both zero-shot and few-shot prompting. This
-version also supports explicitly defining the provided labels with custom
-descriptions. ```ini [components.llm.task] @llm_tasks = "spacy.NER.v2" labels =
-["PERSON", "ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type |
-Default | Description | | ------------------------- | -------------------------
--------------- | -------------------------------------------------------- | ---
+local or through a REST API) more than once. Finally, you can choose to save a
+stringified version of LLM prompts/responses within the `Doc.user_data
+["llm_io"]` attribute by setting `save_io` to `True`. `Doc.user_data["llm_io"]`
+is a dictionary containing one entry for every LLM component within the spaCy
+pipeline. Each entry is itself a dictionary, with two keys: `prompt` and
+`response`. ### Tasks A _task_ defines an NLP problem or question, that will be
+sent to the LLM via a prompt. Further, the task defines how to parse the LLM's
+responses back into structured information. All tasks are registered in spaCy's
+`llm_tasks` registry. Practically speaking, a task should adhere to the
+`Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py). It needs to define
+a `generate_prompts` function and a `parse_responses` function. Moreover, the
+task may define an optional [`scorer` method](https://spacy.io/api/
+scorer#score). It should accept an iterable of `Example`s as input and return a
+score dictionary. If the `scorer` method is defined, `spacy-llm` will call it
+to evaluate the component. #### function `task.generate_prompts` Takes a
+collection of documents, and returns a collection of "prompts", which can be of
+type `Any`. Often, prompts are of type `str` - but this is not enforced to
+allow for maximum flexibility in the framework. | Argument | Type | Description
+| | ----------- | --------------- | ---------------------- | | `docs` |
+`Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
+generated prompts. | #### function `task.parse_responses` Takes a collection of
+LLM responses and the original documents, parses the responses into structured
+information, and sets the annotations on the documents. The `parse_responses`
+function is free to set the annotations in any way, including `Doc` fields like
+`ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
+of type `Iterable[Any]`, though they will often be `str` objects. This depends
+on the return type of the [backend](#backends). | Argument | Type | Description
+| | ----------- | --------------- | ------------------------ | | `docs` |
+`Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
+generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
+| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
+prompting. This version also supports explicitly defining the provided labels
+with custom descriptions. ```ini [components.llm.task] @llm_tasks =
+"spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"] examples = null
+``` | Argument | Type | Default | Description | | ------------------------- | -
+-------------------------------------- | --------------------------------------
+------------------ | ----------------------------------------------------------
 -------------------------------------------------------------------------------
-------------------------------------------------------------------- | |
-`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
-list of labels. | | `template` | `str` | [ner.v2.jinja](./spacy_llm/tasks/
-templates/ner.v2.jinja) | Custom prompt template to send to LLM backend.
-Default templates for each task are located in the `spacy_llm/tasks/templates`
-directory. | | `label_definitions` | `Optional[Dict[str, str]]` | `None` |
-Optional dict mapping a label to a description of that label. These
+------------ | | `labels` | `Union[List[str], str]` | | List of labels or str
+of comma-separated list of labels. | | `template` | `str` | [ner.v2.jinja](./
+spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `label_definitions` | `Optional[Dict[str, str]]` |
+`None` | Optional dict mapping a label to a description of that label. These
 descriptions are added to the prompt to help instruct the LLM on what to
 extract. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
 Optional function that generates examples for few-shot learning. | |
 `normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
 normalizes the labels as returned by the LLM. If `None`, defaults to
 `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
 Alignment mode in case the LLM returns entities that do not align with token
@@ -384,147 +438,226 @@
 "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
 "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
 the REL task relies on pre-extracted entities to make its prediction. Hence,
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
 [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
 "Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
-= "rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
-testing - it tells the LLM to do nothing, and does not set any fields on the
-`docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
-Backends A _backend_ defines which LLM model to query, and how to query it. It
-can be a simple function taking a collection of prompts (consistent with the
-output type of `task.generate_prompts()`) and returning a collection of
-responses (consistent with the expected input of `parse_responses`). Generally
-speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
-but specific implementations can have other signatures, like `Callable[
-[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
-`llm_backends`. If no backend is specified, the repo currently connects to the
-[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
-accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
-third-party libraries in addition to a native REST backend and which should > I
-choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
-prompt management, integration of many different LLM > APIs, and other related
-features such as conversational memory or agents. `spacy-llm` on the other hand
-emphasizes > features we consider useful in the context of NLP pipelines
-utilizing LLMs to process documents (mostly) independent > from each other. It
-makes sense that the feature set of such third-party libraries and `spacy-llm`
-is not identical - > and users might want to take advantage of features not
-available in `spacy-llm`. > > The advantage of offering our own REST backend is
-that we can ensure a larger degree of stability of robustness, as > we can
-guarantee backwards-compatibility and more smoothly integrated error handling.
-> > Ultimately we recommend trying to implement your use case using the REST
-backend first (which is configured as the > default backend). If however there
-are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
-> backend of a third-party library - and easy to customize the prompting
-mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
-to get an API key from openai.com, and ensure that the keys are set as
-environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
-OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
-`requests` and a simple retry mechanism to access an API. ```ini
-[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
-= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
-Default | Description | | ----------- | ---------------- | ------- | ----------
+= "rel_examples.jsonl" ``` #### spacy.Lemma.v1 The `Lemma.v1` task lemmatizes
+the provided text and updates the `lemma_` attribute in the doc's tokens
+accordingly. ```ini [components.llm.task] @llm_tasks = "spacy.Lemma.v1"
+examples = null ``` | Argument | Type | Default | Description | | -------------
+------------ | --------------------------------------- |-----------------------
+------------------------------------| -----------------------------------------
 -------------------------------------------------------------------------------
---------------------------- | | `api` | `str` | | The name of a supported API.
-In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
-| Further configuration passed on to the backend. | | `strict` | `bool` |
-`True` | If `True`, raises an error if the LLM API returns a malformed
-response. Otherwise, return the error responses as is. | | `max_tries` | `int`
-| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
-Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
-following settings can be defined in the `config` dictionary: - `model`: one of
-the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
-`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
-babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
-`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
-For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
-completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
-srush/MiniChain) for the API retrieval part, make sure you have installed it
-first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
-spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
-MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
-blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
-api = "OpenAI" [components.llm.backend.query] @llm_queries =
-"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
---- | -------------------------------------------------------------------------
--------- | ------- | ----------------------------------------------------------
-------------------------- | | `api` | `str` | | The name of an API supported by
-MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
-configuration passed on to the backend. | | `query` | `Optional[Callable[
-["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
-Function that executes the prompts. If `None`, defaults to
-`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
-executes the prompts by running `model(text).run()` for each given textual
-prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
-hwchase17/langchain) for the API retrieval part, make sure you have installed
-it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
-with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
-that LangChain currently only supports Python 3.9 and beyond. Example config
-block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
-= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
-{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
-- | ---------------------------------------------------------------------------
---- | ------- | ---------------------------------------------------------------
---------------------- | | `api` | `str` | | The name of an API supported by
-LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
-configuration passed on to the backend. | | `query` | `Optional[Callable[
-["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
-that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
-The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
-`model(text)` for each given textual prompt. #### spacy.DollyHF.v1 To use this
+----------------------------- | | `template` | `str` | [lemma.jinja](./
+spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
+| `None` | Optional function that generates examples for few-shot learning. |
+`Lemma.v1` prompts the LLM to lemmatize the passed text and return the
+lemmatized version as a list of tokens and their corresponding lemma. E. g. the
+text `I'm buying ice cream for my friends` should invoke the response ``` I: I
+'m: be buying: buy ice: ice cream: cream for: for my: my friends: friend .: .
+``` If for any given text/doc instance the number of lemmas returned by the LLM
+doesn't match the number of tokens recognized by spaCy, no lemmas are stored in
+the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is
+updated with the lemma suggested by the LLM. To perform few-shot learning, you
+can write down a few examples in a separate file, and provide these to be
+injected into the prompt to the LLM. The default reader
+`spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+```yaml - text: I'm buying ice cream. lemmas: - "I": "I" - "'m": "be" -
+"buying": "buy" - "ice": "ice" - "cream": "cream" - ".": "." - text: I've
+watered the plants. lemmas: - "I": "I" - "'ve": "have" - "watered": "water" -
+"the": "the" - "plants": "plant" - ".": "." ``` ```ini [components.llm.task]
+@llm_tasks = "spacy.Lemma.v1" [components.llm.task.examples] @misc =
+"spacy.FewShotReader.v1" path = "lemma_examples.yml" ``` #### spacy.NoOp.v1
+This task is only useful for testing - it tells the LLM to do nothing, and does
+not set any fields on the `docs`. ```ini [components.llm.task] @llm_tasks =
+"spacy.NoOp.v1" ``` ### Backends A _backend_ defines which LLM model to query,
+and how to query it. It can be a simple function taking a collection of prompts
+(consistent with the output type of `task.generate_prompts()`) and returning a
+collection of responses (consistent with the expected input of
+`parse_responses`). Generally speaking, it's a function of type `Callable[
+[Iterable[Any]], Iterable[Any]]`, but specific implementations can have other
+signatures, like `Callable[[Iterable[str]], Iterable[str]]`. All built-in
+backends are registered in `llm_backends`. If no backend is specified, the repo
+currently connects to the [`OpenAI` API](#openai) by default, using the built-
+in REST protocol, and accesses the `"gpt-3.5-turbo"` model. > :question: _Why
+are there backends for third-party libraries in addition to a native REST
+backend and which should > I choose?_ > > Third-party libraries like
+`langchain` or `minichain` focus on prompt management, integration of many
+different LLM > APIs, and other related features such as conversational memory
+or agents. `spacy-llm` on the other hand emphasizes > features we consider
+useful in the context of NLP pipelines utilizing LLMs to process documents
+(mostly) independent > from each other. It makes sense that the feature set of
+such third-party libraries and `spacy-llm` is not identical - > and users might
+want to take advantage of features not available in `spacy-llm`. > > The
+advantage of offering our own REST backend is that we can ensure a larger
+degree of stability of robustness, as > we can guarantee backwards-
+compatibility and more smoothly integrated error handling. > > Ultimately we
+recommend trying to implement your use case using the REST backend first (which
+is configured as the > default backend). If however there are features or APIs
+not covered by `spacy-llm`, it's trivial to switch to the > backend of a third-
+party library - and easy to customize the prompting mechanism, if so required.
+#### OpenAI When the backend uses OpenAI, you have to get an API key from
+openai.com, and ensure that the keys are set as environmental variables:
+```shell export OPENAI_API_KEY="sk-..." export OPENAI_API_ORG="org-..." ```
+#### spacy.REST.v1 This default backend uses `requests` and a simple retry
+mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
+"spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-turbo",
+"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
+-- | ---------------- | ------- | ---------------------------------------------
+----------------------------------------------------------------------- | |
+`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
+supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
+passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
+error if the LLM API returns a malformed response. Otherwise, return the error
+responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
+request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
+When `api` is set to `OpenAI`, the following settings can be defined in the
+`config` dictionary: - `model`: one of the following list of supported models:
+- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
+turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
+- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
+`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
+api.openai.com/v1/completions`. For models requiring the chat endpoint, use
+`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
+[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
+make sure you have installed it first: ```shell python -m pip install
+"minichain>=0.3,<0.4" # Or install with spacy-llm directly python -m pip
+install "spacy-llm[minichain]" ``` Note that MiniChain currently only supports
+Python 3.8, 3.9 and 3.10. Example config blocks: ```ini
+[components.llm.backend] @llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
+[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
+Argument | Type | Default | Description | | -------- | ------------------------
+--------------------------------------------------------- | ------- | ---------
+-------------------------------------------------------------------------- | |
+`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
+`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
+backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
+Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
+If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
+(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
+for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
+(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
+you have installed it first: ```shell python -m pip install
+"langchain>=0.0.144,<0.1" # Or install with spacy-llm directly python -m pip
+install "spacy-llm[langchain]" ``` Note that LangChain currently only supports
+Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
+@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
+"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
+Default | Description | | -------- | ------------------------------------------
+------------------------------------ | ------- | ------------------------------
+------------------------------------------------------ | | `api` | `str` | |
+The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
+[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
+`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
+Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
+defaults to `spacy.CallLangChain.v1`. | The default `query`
+(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
+each given textual prompt. #### spacy.Dolly_HF.v1 To use this backend, ideally
+you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
+your virtual environment. This allows you to have the setting `device=cuda:0`
+in your config, which ensures that the model is loaded entirely on the GPU (and
+fails otherwise). You can do so with ```shell python -m pip install "spacy-llm
+[transformers]" "transformers[sentencepiece]" ``` If you don't have access to a
+GPU, you can install `accelerate` and set`device_map=auto` instead, but be
+aware that this may result in some layers getting distributed to the CPU or
+even the hard drive, which may ultimately result in extremely slow queries.
+```shell python -m pip install "accelerate>=0.16.0,<1.0" ``` Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1"
+model = "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description
+| | ------------- | ---------------- | ------- | ------------------------------
+------------------------------------------------------------------ | | `model`
+| `str` | | The name of a Dolly model that is supported. | | `config_init` |
+`Dict[str, Any]` | `{}` | Further configuration passed on to the construction
+of the model with `transformers.pipeline()`. | | `config_run` | `Dict[str,
+Any]` | `{}` | Further configuration used during model inference. | Supported
+models (see the [Databricks models page](https://huggingface.co/databricks) on
+Hugging Face for details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-
+v2-7b"` - `"databricks/dolly-v2-12b"` Note that Hugging Face will download this
+model the first time you use it - you can [define the cached directory](https:/
+/huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting
+the environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
 backend, ideally you have a GPU enabled and have installed `transformers`,
-`torch` and CUDA in your virtual environment. This allows you to have the
-setting `device=cuda:0` in your config, which ensures that the model is loaded
-entirely on the GPU (and fails otherwise). ```shell python -m pip install
-"torch>=1.13.1,<2.0" python -m pip install "transformers>=4.28.1,<5.0" # Or
-install with spacy-llm directly python -m pip install "spacy-llm[transformers]"
+`torch` and CUDA in your virtual environment. You can do so with ```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ``` If you don't have access to a GPU, you can install `accelerate` and
 set`device_map=auto` instead, but be aware that this may result in some layers
 getting distributed to the CPU or even the hard drive, which may ultimately
 result in extremely slow queries. ```shell python -m pip install
 "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
-[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" model =
-"databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
----- | ---------------- | ------- | -------------------------------------------
------------------------------------------------------ | | `model` | `str` | |
-The name of a Dolly model that is supported. | | `config` | `Dict[Any, Any]` |
-`{}` | Further configuration passed on to the construction of the model with
-`transformers.pipeline()`. | Supported models (see the [Databricks models page]
-(https://huggingface.co/databricks) on Hugging Face for details): -
-`"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` - `"databricks/dolly-
-v2-12b"` Note that Hugging Face will download this model the first time you use
-it - you can [define the cached directory](https://huggingface.co/docs/
+[components.llm.backend] @llm_backends = "spacy.StableLM_HF.v1" model =
+"stabilityai/stablelm-tuned-alpha-7b" ``` | Argument | Type | Default |
+Description | | ------------- | ---------------- | ------- | ------------------
+-------------------------------------------------------------------------------
+--------------------------- | | `model` | `str` | | The name of a StableLM
+model that is supported. | | `config_init` | `Dict[str, Any]` | `{}` | Further
+configuration passed on to the construction of the model with
+`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
+[str, Any]` | `{}` | Further configuration used during model inference. |
+Supported models (see the [Stability AI StableLM GitHub repo](https://
+github.com/Stability-AI/StableLM/#stablelm-alpha) for details): -
+`"stabilityai/stablelm-base-alpha-3b"` - `"stabilityai/stablelm-base-alpha-7b"`
+- `"stabilityai/stablelm-tuned-alpha-3b"` - `"stabilityai/stablelm-tuned-alpha-
+7b"` Note that Hugging Face will download this model the first time you use it
+- you can [define the cached directory](https://huggingface.co/docs/
 huggingface_hub/main/en/guides/manage-cache) by setting the environmental
-variable `HF_HOME`. ### Cache Interacting with LLMs, either through an external
-API or a local instance, is costly. Since developing an NLP pipeline generally
-means a lot of exploration and prototyping, `spacy-llm` implements a built-in
-cache to avoid reprocessing the same documents at each run. Example config
-block: ```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1", path =
-"path/to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
-Default | Description | | -------------------- | ---------------------------- |
-------- | ---------------------------------------------------- | | `path` |
-`Optional[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching
-is performed. | | `batch_size` | `int` | 64 | Number of docs in one batch
-(file). | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
-in memory. | Note that since the cache is generated by a registered function,
-you can also provide your own registered function returning your own cache
-implementation. If you wish to do so, ensure that your cache object adheres to
-the `Protocol` defined in `spacy_llm.ty.Cache`. ### Various functions ####
-spacy.FewShotReader.v1 This function is registered in spaCy's `misc` registry,
-and reads in examples from a `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses
-[`srsly`](https://github.com/explosion/srsly) to read in these files and parses
-them depending on the file extension. ```ini [components.llm.task.examples]
-@misc = "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument |
-Type | Description | | -------- | ------------------ | ------------------------
--------------------------------------------------- | | `path` | `Union[str,
-Path]` | Path to an examples file with suffix `.yml`, `.yaml`, `.json` or
-`.jsonl`. | #### spacy.FileReader.v1 This function is registered in spaCy's
-`misc` registry, and reads a file provided to the `path` to return a `str`
+variable `HF_HOME`. #### spacy.OpenLLaMaHF.v1 To use this backend, ideally you
+have a GPU enabled and have installed - `transformers[sentencepiece]` - `torch`
+- CUDA in your virtual environment. You can do so with ```shell python -m pip
+install "spacy-llm[transformers]" "transformers[sentencepiece]" ``` If you
+don't have access to a GPU, you can install `accelerate` and
+set`device_map=auto` instead, but be aware that this may result in some layers
+getting distributed to the CPU or even the hard drive, which may ultimately
+result in extremely slow queries. ```shell python -m pip install
+"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.backend] @llm_backends = "spacy.OpenLLaMaHF.v1" model =
+"openlm-research/open_llama_3b_350bt_preview" ``` | Argument | Type | Default |
+Description | | ------------- | ---------------- | ------- | ------------------
+-------------------------------------------------------------------------------
+--------------------------- | | `model` | `str` | | The name of a OpenLLaMa
+model that is supported. | | `config_init` | `Dict[str, Any]` | `{}` | Further
+configuration passed on to the construction of the model with
+`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
+[str, Any]` | `{}` | Further configuration used during model inference. |
+Supported models (see the [OpenLM Research OpenLLaMa GitHub repo](https://
+github.com/openlm-research/open_llama) for details): - `"openlm-research/
+open_llama_3b_350bt_preview"` - `"openlm-research/open_llama_3b_600bt_preview"`
+- `"openlm-research/open_llama_7b_400bt_preview"` - `"openlm-research/
+open_llama_7b_700bt_preview"` Note that Hugging Face will download this model
+the first time you use it - you can [define the cached directory](https://
+huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
+environmental variable `HF_HOME`. ### Cache Interacting with LLMs, either
+through an external API or a local instance, is costly. Since developing an NLP
+pipeline generally means a lot of exploration and prototyping, `spacy-llm`
+implements a built-in cache to avoid reprocessing the same documents at each
+run. Example config block: ```ini [components.llm.cache] @llm_misc =
+"spacy.BatchCache.v1", path = "path/to/cache" batch_size = 64
+max_batches_in_mem = 4 ``` | Argument | Type | Default | Description | | ------
+-------------- | ---------------------------- | ------- | ---------------------
+------------------------------- | | `path` | `Optional[Union[str, Path]]` |
+`None` | Cache directory. If `None`, no caching is performed. | | `batch_size`
+| `int` | 64 | Number of docs in one batch (file). | | `max_batches_in_mem` |
+`int` | 4 | Max. number of batches to hold in memory. | Note that since the
+cache is generated by a registered function, you can also provide your own
+registered function returning your own cache implementation. If you wish to do
+so, ensure that your cache object adheres to the `Protocol` defined in
+`spacy_llm.ty.Cache`. ### Various functions #### spacy.FewShotReader.v1 This
+function is registered in spaCy's `misc` registry, and reads in examples from a
+`.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
+github.com/explosion/srsly) to read in these files and parses them depending on
+the file extension. ```ini [components.llm.task.examples] @misc =
+"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument | Type |
+Description | | -------- | ------------------ | -------------------------------
+------------------------------------------- | | `path` | `Union[str, Path]` |
+Path to an examples file with suffix `.yml`, `.yaml`, `.json` or `.jsonl`. |
+#### spacy.FileReader.v1 This function is registered in spaCy's `misc`
+registry, and reads a file provided to the `path` to return a `str`
 representation of its contents. This function is typically used to read [Jinja]
 (https://jinja.palletsprojects.com/en/3.1.x/) files containing the prompt
 template. ```ini [components.llm.task.template] @misc = "spacy.FileReader.v1"
 path = "ner_template.jinja2" ``` | Argument | Type | Description | | -------- |
 ------------------ | ---------------------------- | | `path` | `Union[str,
 Path]` | Path to the file to be read. | #### Normalizer functions These
 functions provide simple normalizations for string comparisons, e.g. between a
```

### Comparing `spacy-llm-0.2.1/pyproject.toml` & `spacy-llm-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/setup.cfg` & `spacy-llm-0.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.2.1
+version = 0.3.0
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -42,15 +42,15 @@
 	spacy.FewShotReader.v1 = spacy_llm.registry:fewshot_reader
 	spacy.FileReader.v1 = spacy_llm.registry:file_reader
 
 [options.extras_require]
 minichain = 
 	minichain>=0.3,<0.4
 langchain = 
-	langchain>=0.0.180,<0.0.185
+	langchain==0.0.191
 transformers = 
 	torch>=1.13.1,<2.0
 	transformers>=4.28.1,<5.0
 
 [bdist_wheel]
 universal = true
```

### Comparing `spacy-llm-0.2.1/spacy_llm/backends/integration/base.py` & `spacy-llm-0.3.0/spacy_llm/backends/integration/remote/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Iterable, TypeVar, Callable, Any
+from typing import Any, Callable, Iterable, TypeVar
 
 # Type of prompts returned from Task.generate_prompts().
 _PromptType = TypeVar("_PromptType")
 # Type of responses returned from query function.
 _ResponseType = TypeVar("_ResponseType")
 
 
-class Backend:
+class RemoteBackend:
     def __init__(
         self,
         integration: Any,
         query: Callable[[Any, Iterable[_PromptType]], Iterable[_ResponseType]],
     ):
-        """Initializes Backend instance.
+        """Initializes Backend instance for remote APIs.
         integration (Any): Object/Callable enabling LLM calls through third-party libraries. This can be a HuggingFace
             model, a LangChain API class, or anything else able to execute LLM prompts directly or indirectly.
         query (Callable[[Any, Iterable[_PromptType]], Iterable[_ResponseType]]): Callable executing LLM prompts when
             supplied with the `integration` object.
         """
-        self.integration = integration
+        self._integration = integration
         self.query = query
 
     def __call__(self, prompts: Iterable[_PromptType]) -> Iterable[_ResponseType]:
         """Executes prompts on specified API.
         prompts (Iterable[_PromptType]): Prompts to execute.
-        RETURNS (Iterable[__ResponseType]): API responses.
+        RETURNS (Iterable[_ResponseType]): API responses.
         """
-        return self.query(self.integration, prompts)
+        return self.query(self._integration, prompts)
```

### Comparing `spacy-llm-0.2.1/spacy_llm/backends/integration/langchain.py` & `spacy-llm-0.3.0/spacy_llm/backends/integration/remote/langchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Any, Callable, Dict, Iterable, Optional, Type
 
 from spacy.util import SimpleFrozenDict
 
-from . import Backend
-from ...compat import has_langchain, langchain
-from ...registry import registry
+from ....compat import has_langchain, langchain
+from ....registry import registry
+from . import RemoteBackend
 
 
 def _check_installation() -> None:
     """Checks whether `langchain` is installed. Raises an error otherwise."""
     if not has_langchain:
         raise ValueError(
             "The LangChain backend requires `langchain` to be installed, which it is not. See "
             "https://github.com/hwchase17/langchain for installation instructions."
         )
 
 
 @registry.llm_queries("spacy.CallLangChain.v1")
-def query_langchain() -> Callable[
-    ["langchain.llms.base.BaseLLM", Iterable[Any]], Iterable[Any]
-]:
+def query_langchain() -> (
+    Callable[["langchain.llms.base.BaseLLM", Iterable[Any]], Iterable[Any]]
+):
     """Returns query Callable for LangChain.
     RETURNS (Callable[["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]:): Callable executing simple prompts on
         the specified LangChain backend.
     """
     return _prompt_langchain
 
 
@@ -60,15 +60,15 @@
     api = api.lower()
     type_to_cls_dict: Dict[
         str, Type[langchain.llms.base.BaseLLM]
     ] = langchain.llms.type_to_cls_dict
 
     if api in type_to_cls_dict:
         model = config.pop("model")
-        return Backend(
+        return RemoteBackend(
             integration=type_to_cls_dict[api](model_name=model, **config),
             query=query_langchain() if query is None else query,
         )
     else:
         raise KeyError(
             f"The requested API {api} is not available in `langchain.llms.type_to_cls_dict`."
         )
```

### Comparing `spacy-llm-0.2.1/spacy_llm/backends/integration/minichain.py` & `spacy-llm-0.3.0/spacy_llm/backends/integration/remote/minichain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Callable, Dict, Iterable, Optional
 
 from spacy.util import SimpleFrozenDict
 
-from . import Backend
-from ...compat import has_minichain, minichain
-from ...registry import registry
+from ....compat import has_minichain, minichain
+from ....registry import registry
+from .base import RemoteBackend
 
 
 def _check_installation() -> None:
     """Checks whether `minichain` is installed. Raises an error otherwise."""
     if not has_minichain:
         raise ValueError(
             "The MiniChain backend requires `minichain` to be installed, which it is not. See "
@@ -56,15 +56,15 @@
     """
     _check_installation()
 
     if "model" not in config:
         raise ValueError("The LLM model must be specified in the config.")
 
     if hasattr(minichain.backend, api):
-        return Backend(
+        return RemoteBackend(
             integration=getattr(minichain.backend, api)(**config),
             query=query_minichain() if query is None else query,
         )
     else:
         raise KeyError(
             f"The requested API {api} is not available in `minichain.backend`."
         )
```

### Comparing `spacy-llm-0.2.1/spacy_llm/backends/rest/backend/base.py` & `spacy-llm-0.3.0/spacy_llm/backends/rest/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/backends/rest/backend/noop.py` & `spacy-llm-0.3.0/spacy_llm/backends/rest/noop.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import time
 from typing import Dict, Iterable
 
 from .base import Backend
 
+_NOOP_RESPONSE = ""
+
 
 class NoOpBackend(Backend):
     """NoOp backend. Used for tests."""
 
     _CALL_TIMEOUT = 0.01
 
     @property
@@ -16,8 +18,8 @@
     @property
     def credentials(self) -> Dict[str, str]:
         return {}
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         # Assume time penalty for API calls.
         time.sleep(NoOpBackend._CALL_TIMEOUT)
-        return [""] * len(list(prompts))
+        return [_NOOP_RESPONSE] * len(list(prompts))
```

### Comparing `spacy-llm-0.2.1/spacy_llm/backends/rest/backend/openai.py` & `spacy-llm-0.3.0/spacy_llm/backends/rest/openai.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/backends/rest/registry.py` & `spacy-llm-0.3.0/spacy_llm/backends/rest/registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-from typing import Any, Callable, Dict, Iterable
+from typing import Any, Callable, Dict, Iterable, Type
+
 
 from spacy.util import SimpleFrozenDict
 
-from .backend import supported_apis
+from . import anthropic, base, openai, noop
 from ...registry import registry
 
 
+supported_apis: Dict[str, Type[base.Backend]] = {
+    "OpenAI": openai.OpenAIBackend,
+    "Anthropic": anthropic.AnthropicBackend,
+    "NoOp": noop.NoOpBackend,
+}
+
+
 @registry.llm_backends("spacy.REST.v1")
 def backend_rest(
     api: str,
     config: Dict[Any, Any] = SimpleFrozenDict(),
     strict: bool = True,
     max_tries: int = 5,
     interval: float = 1.0,
```

### Comparing `spacy-llm-0.2.1/spacy_llm/cache.py` & `spacy-llm-0.3.0/spacy_llm/cache.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Dict, Iterable, List, Optional, Union
-import numpy
 
+import numpy
 import srsly  # type: ignore[import]
 from spacy.tokens import Doc, DocBin
 from spacy.vocab import Vocab
 
 from .registry import registry
```

### Comparing `spacy-llm-0.2.1/spacy_llm/compat.py` & `spacy-llm-0.3.0/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/pipeline/llm.py` & `spacy-llm-0.3.0/spacy_llm/pipeline/llm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+import logging
+from collections import defaultdict
+from itertools import tee
 from pathlib import Path
 from typing import Dict, Iterable, Iterator, List, Optional, Tuple, Union, cast
 
 import spacy
+from spacy import util
 from spacy.language import Language
 from spacy.pipeline import Pipe
 from spacy.tokens import Doc
 from spacy.training import Example
+from spacy.ty import InitializableComponent as Initializable
 from spacy.vocab import Vocab
 
 from .. import registry  # noqa: F401
 from ..compat import TypedDict
-from ..ty import Cache, LLMTask, PromptExecutor, validate_types
+from ..ty import Cache, LLMTask, PromptExecutor, Scorable, Serializable, validate_types
+
+logger = logging.getLogger("spacy_llm")
+logger.addHandler(logging.NullHandler())
 
 
 class CacheConfigType(TypedDict):
     path: Optional[Path]
     batch_size: int
     max_batches_in_mem: int
 
@@ -33,43 +41,47 @@
         },
         "cache": {
             "@llm_misc": "spacy.BatchCache.v1",
             "path": None,
             "batch_size": 64,
             "max_batches_in_mem": 4,
         },
+        "save_io": False,
     },
 )
 def make_llm(
     nlp: Language,
     name: str,
     task: Optional[LLMTask],
     backend: PromptExecutor,
     cache: Cache,
+    save_io: bool,
 ) -> "LLMWrapper":
     """Construct an LLM component.
 
     nlp (Language): Pipeline.
     name (str): The component instance name, used to add entries to the
         losses during training.
     task (Optional[LLMTask]): An LLMTask can generate prompts for given docs, and can parse the LLM's responses into
         structured information and set that back on the docs.
     backend (Callable[[Iterable[Any]], Iterable[Any]]]): Callable querying the specified LLM API.
     cache (Cache): Cache to use for caching prompts and responses per doc (batch).
+    save_io (bool): Whether to save LLM I/O (prompts and responses) in the `Doc._.llm_io` custom extension.
     """
     if task is None:
         raise ValueError(
             "Argument `task` has not been specified, but is required (e. g. {'@llm_tasks': "
             "'spacy.NER.v2'})."
         )
     validate_types(task, backend)
 
     return LLMWrapper(
         name=name,
         task=task,
+        save_io=save_io,
         backend=backend,
         cache=cache,
         vocab=nlp.vocab,
     )
 
 
 class LLMWrapper(Pipe):
@@ -79,31 +91,40 @@
         self,
         name: str = "LLMWrapper",
         *,
         vocab: Vocab,
         task: LLMTask,
         backend: PromptExecutor,
         cache: Cache,
+        save_io: bool,
     ) -> None:
         """
         Component managing execution of prompts to LLM APIs and mapping responses back to Doc/Span instances.
 
         name (str): The component instance name, used to add entries to the
             losses during training.
         vocab (Vocab): Pipeline vocabulary.
         task (Optional[LLMTask]): An LLMTask can generate prompts for given docs, and can parse the LLM's responses into
             structured information and set that back on the docs.
         backend (Callable[[Iterable[Any]], Iterable[Any]]]): Callable querying the specified LLM API.
         cache (Cache): Cache to use for caching prompts and responses per doc (batch).
+        save_io (bool): Whether to save LLM I/O (prompts and responses) in the `Doc._.llm_io` custom extension.
         """
         self._name = name
         self._task = task
         self._backend = backend
         self._cache = cache
         self._cache.vocab = vocab
+        self._save_io = save_io
+
+        # This is done this way because spaCy's `validate_init_settings` function
+        # does not support `**kwargs: Any`.
+        # See https://github.com/explosion/spaCy/blob/master/spacy/schemas.py#L111
+        if isinstance(self._task, Initializable):
+            self.initialize = self._task.initialize
 
     def __call__(self, doc: Doc) -> Doc:
         """Apply the LLM wrapper to a Doc instance.
 
         doc (Doc): The Doc instance to process.
         RETURNS (Doc): The processed Doc.
         """
@@ -117,15 +138,15 @@
         """Score a batch of examples.
 
         examples (Iterable[Example]): The examples to score.
         RETURNS (Dict[str, Any]): The scores.
 
         DOCS: https://spacy.io/api/pipe#score
         """
-        if hasattr(self._task, "scorer") and self._task.scorer is not None:
+        if isinstance(self._task, Scorable):
             return self._task.scorer(examples)
         return {}
 
     def pipe(self, stream: Iterable[Doc], *, batch_size: int = 128) -> Iterator[Doc]:
         """Apply the LLM prompt to a stream of documents.
 
         stream (Iterable[Doc]): A stream of documents.
@@ -144,58 +165,131 @@
         If a cache is configured, only sends prompts to backend for docs not found in cache.
 
         docs (List[Doc]): Input batch of docs
         RETURNS (List[Doc]): Processed batch of docs with task annotations set
         """
         is_cached = [doc in self._cache for doc in docs]
         noncached_doc_batch = [doc for i, doc in enumerate(docs) if not is_cached[i]]
-        prompts = self._task.generate_prompts(noncached_doc_batch)
-        responses = self._backend(prompts)
-        modified_docs = iter(self._task.parse_responses(noncached_doc_batch, responses))
+        if len(noncached_doc_batch) < len(docs):
+            logger.debug(
+                "Found %d docs in cache. Processing %d docs not found in cache",
+                len(docs) - len(noncached_doc_batch),
+                len(noncached_doc_batch),
+            )
+
+        modified_docs: Iterator[Doc] = iter(())
+        if len(noncached_doc_batch) > 0:
+            n_iters = 3 if self._save_io else 2
+            prompts_iters = tee(
+                self._task.generate_prompts(noncached_doc_batch), n_iters
+            )
+            responses_iters = tee(self._backend(prompts_iters[0]), n_iters)
+            for prompt, response, doc in zip(
+                prompts_iters[1], responses_iters[1], noncached_doc_batch
+            ):
+                logger.debug("Generated prompt for doc: %s\n%s", doc.text, prompt)
+                logger.debug("LLM response for doc: %s\n%s", doc.text, response)
+
+            modified_docs = iter(
+                self._task.parse_responses(noncached_doc_batch, responses_iters[0])
+            )
+
         final_docs = []
         for i, doc in enumerate(docs):
             if is_cached[i]:
                 cached_doc = self._cache[doc]
                 assert cached_doc is not None
                 final_docs.append(cached_doc)
             else:
                 doc = next(modified_docs)
                 self._cache.add(doc)
                 final_docs.append(doc)
 
+                if self._save_io:
+                    # Make sure the `llm_io` field is set
+                    doc.user_data["llm_io"] = doc.user_data.get(
+                        "llm_io", defaultdict(dict)
+                    )
+                    llm_io = doc.user_data["llm_io"][self._name]
+                    llm_io["prompt"] = str(next(prompts_iters[2]))
+                    llm_io["response"] = str(next(responses_iters[2]))
+
         return final_docs
 
-    def to_bytes(self, *, exclude: Tuple[str] = cast(Tuple[str], tuple())) -> bytes:
+    def to_bytes(
+        self,
+        *,
+        exclude: Tuple[str] = cast(Tuple[str], tuple()),
+    ) -> bytes:
         """Serialize the LLMWrapper to a bytestring.
 
         exclude (Tuple): Names of properties to exclude from serialization.
         RETURNS (bytes): The serialized object.
         """
-        return b""
 
-    def from_bytes(self, bytes_data: bytes, *, exclude=tuple()) -> "LLMWrapper":
+        serialize = {}
+
+        if isinstance(self._task, Serializable):
+            serialize["task"] = lambda: self._task.to_bytes(exclude=exclude)  # type: ignore[attr-defined]
+        if isinstance(self._backend, Serializable):
+            serialize["backend"] = lambda: self._backend.to_bytes(exclude=exclude)  # type: ignore[attr-defined]
+
+        return util.to_bytes(serialize, exclude)
+
+    def from_bytes(
+        self,
+        bytes_data: bytes,
+        *,
+        exclude: Tuple[str] = cast(Tuple[str], tuple()),
+    ) -> "LLMWrapper":
         """Load the LLMWrapper from a bytestring.
 
         bytes_data (bytes): The data to load.
-        exclude (Tuple): Names of properties to exclude from deserialization.
+        exclude (Tuple[str]): Names of properties to exclude from deserialization.
         RETURNS (LLMWrapper): Modified LLMWrapper instance.
         """
+
+        deserialize = {}
+
+        if isinstance(self._task, Serializable):
+            deserialize["task"] = lambda b: self._task.from_bytes(b, exclude=exclude)  # type: ignore[attr-defined]
+        if isinstance(self._backend, Serializable):
+            deserialize["backend"] = lambda b: self._backend.from_bytes(b, exclude=exclude)  # type: ignore[attr-defined]
+
+        util.from_bytes(bytes_data, deserialize, exclude)
         return self
 
     def to_disk(
         self, path: Path, *, exclude: Tuple[str] = cast(Tuple[str], tuple())
     ) -> None:
         """Serialize the LLMWrapper to disk.
         path (Path): A path (currently unused).
         exclude (Tuple): Names of properties to exclude from serialization.
         """
-        return None
+
+        serialize = {}
+
+        if isinstance(self._task, Serializable):
+            serialize["task"] = lambda p: self._task.to_disk(p, exclude=exclude)  # type: ignore[attr-defined]
+        if isinstance(self._backend, Serializable):
+            serialize["backend"] = lambda p: self._backend.to_disk(p, exclude=exclude)  # type: ignore[attr-defined]
+
+        return util.to_disk(path, serialize, exclude)
 
     def from_disk(
         self, path: Path, *, exclude: Tuple[str] = cast(Tuple[str], tuple())
     ) -> "LLMWrapper":
         """Load the LLMWrapper from disk.
         path (Path): A path (currently unused).
         exclude (Tuple): Names of properties to exclude from deserialization.
         RETURNS (LLMWrapper): Modified LLMWrapper instance.
         """
+
+        serialize = {}
+
+        if isinstance(self._task, Serializable):
+            serialize["task"] = lambda p: self._task.from_disk(p, exclude=exclude)  # type: ignore[attr-defined]
+        if isinstance(self._backend, Serializable):
+            serialize["backend"] = lambda p: self._backend.from_disk(p, exclude=exclude)  # type: ignore[attr-defined]
+
+        util.from_disk(path, serialize, exclude)
         return self
```

### Comparing `spacy-llm-0.2.1/spacy_llm/registry/normalizer.py` & `spacy-llm-0.3.0/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/registry/reader.py` & `spacy-llm-0.3.0/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/__init__.py` & `spacy-llm-0.3.0/spacy_llm/tasks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from .lemma import LemmaTask, make_lemma_task
 from .ner import NERTask, make_ner_task, make_ner_task_v2
 from .noop import NoopTask, make_noop_task
-from .rel import RELTask
+from .rel import RELTask, make_rel_task
 from .spancat import SpanCatTask, make_spancat_task, make_spancat_task_v2
 from .textcat import TextCatTask, make_textcat_task
 
 __all__ = [
-    "NoopTask",
-    "NERTask",
-    "SpanCatTask",
-    "TextCatTask",
+    "make_lemma_task",
     "make_ner_task",
     "make_ner_task_v2",
     "make_noop_task",
+    "make_rel_task",
     "make_spancat_task",
     "make_spancat_task_v2",
     "make_textcat_task",
-    "TextCatTask",
-    "SpanCatTask",
+    "LemmaTask",
+    "NERTask",
+    "NoopTask",
     "RELTask",
+    "SpanCatTask",
+    "TextCatTask",
 ]
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/templates/ner.jinja` & `spacy-llm-0.3.0/spacy_llm/tasks/templates/ner.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy-llm-0.3.0/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/templates/rel.jinja` & `spacy-llm-0.3.0/spacy_llm/tasks/templates/rel.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/templates/spancat.jinja` & `spacy-llm-0.3.0/spacy_llm/tasks/templates/spancat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy-llm-0.3.0/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.jinja` & `spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/templates/textcat.v3.jinja` & `spacy-llm-0.3.0/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/textcat.py` & `spacy-llm-0.3.0/spacy_llm/tasks/rel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,227 +1,225 @@
-from typing import Any, Callable, Dict, Iterable, List, Optional, Union
+from typing import Callable, Dict, Iterable, List, Optional, Type, Union
 
 import jinja2
-from pydantic import BaseModel
-from spacy.scorer import Scorer
+from pydantic import BaseModel, Field, ValidationError, validator
+from spacy.language import Language
 from spacy.tokens import Doc
 from spacy.training import Example
 from wasabi import msg
 
 from ..registry import lowercase_normalizer, registry
 from ..ty import ExamplesConfigType
 from ..util import split_labels
 from .templates import read_template
+from .util import SerializableTask
 
-_DEFAULT_TEXTCAT_TEMPLATE_V1 = read_template("textcat")
-_DEFAULT_TEXTCAT_TEMPLATE_V2 = read_template("textcat.v2")
-_DEFAULT_TEXTCAT_TEMPLATE_V3 = read_template("textcat.v3")
 
+class RelationItem(BaseModel):
+    dep: int
+    dest: int
+    relation: str
 
-class TextCatExample(BaseModel):
+    @validator("dep", "dest", pre=True)
+    def clean_ent(cls, value):
+        if isinstance(value, str):
+            value = value.strip("ENT")
+        return value
+
+
+class EntityItem(BaseModel):
+    start_char: int
+    end_char: int
+    label_: str = Field(alias="label")
+
+
+class RELExample(BaseModel):
     text: str
-    answer: str
+    ents: List[EntityItem]
+    relations: List[RelationItem]
 
 
-@registry.llm_tasks("spacy.TextCat.v1")
-def make_textcat_task(
-    labels: str,
-    examples: ExamplesConfigType = None,
-    normalizer: Optional[Callable[[str], str]] = None,
-    exclusive_classes: bool = False,
-    allow_none: bool = True,
-    verbose: bool = False,
-) -> "TextCatTask":
-    labels_list = split_labels(labels)
-    raw_examples = examples() if callable(examples) else examples
-    textcat_examples = (
-        [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
-    )
-    return TextCatTask(
-        labels=labels_list,
-        template=_DEFAULT_TEXTCAT_TEMPLATE_V1,
-        examples=textcat_examples,
-        normalizer=normalizer,
-        exclusive_classes=exclusive_classes,
-        allow_none=allow_none,
-        verbose=verbose,
-    )
+def _preannotate(doc: Union[Doc, RELExample]) -> str:
+    """Creates a text version of the document with annotated entities."""
+    offset = 0
 
+    text = doc.text
 
-@registry.llm_tasks("spacy.TextCat.v2")
-def make_textcat_task_v2(
-    labels: Union[List[str], str],
-    template: str = _DEFAULT_TEXTCAT_TEMPLATE_V2,
-    examples: ExamplesConfigType = None,
-    normalizer: Optional[Callable[[str], str]] = None,
-    exclusive_classes: bool = False,
-    allow_none: bool = True,
-    verbose: bool = False,
-) -> "TextCatTask":
-    labels_list = split_labels(labels)
-    raw_examples = examples() if callable(examples) else examples
-    textcat_examples = (
-        [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
-    )
-    return TextCatTask(
-        labels=labels_list,
-        template=template,
-        examples=textcat_examples,
-        normalizer=normalizer,
-        exclusive_classes=exclusive_classes,
-        allow_none=allow_none,
-        verbose=verbose,
-    )
+    for i, ent in enumerate(doc.ents):
+        end = ent.end_char
+        before, after = text[: end + offset], text[end + offset :]
+
+        annotation = f"[ENT{i}:{ent.label_}]"
+        offset += len(annotation)
 
+        text = f"{before}{annotation}{after}"
 
-@registry.llm_tasks("spacy.TextCat.v3")
-def make_textcat_task_v3(
-    labels: Union[List[str], str],
-    template: str = _DEFAULT_TEXTCAT_TEMPLATE_V3,
+    return text
+
+
+_DEFAULT_REL_TEMPLATE = read_template("rel")
+
+
+@registry.llm_tasks("spacy.REL.v1")
+def make_rel_task(
+    labels: Union[List[str], str] = [],
+    template: str = _DEFAULT_REL_TEMPLATE,
     label_definitions: Optional[Dict[str, str]] = None,
     examples: ExamplesConfigType = None,
     normalizer: Optional[Callable[[str], str]] = None,
-    exclusive_classes: bool = False,
-    allow_none: bool = True,
     verbose: bool = False,
-) -> "TextCatTask":
+) -> "RELTask":
+    """REL.v1 task factory.
+
+    The REL task populates a `Doc._.rel` custom attribute.
+
+    labels (List[str]): List of labels to pass to the template,
+        either an actual list or a comma-separated string.
+        Leave empty to populate it at initialization time (only if examples are provided).
+    template (str): Prompt template passed to the model.
+    label_definitions (Optional[Dict[str, str]]): Map of label -> description
+        of the label to help the language model output the entities wanted.
+        It is usually easier to provide these definitions rather than
+        full examples, although both can be provided.
+    examples (Optional[Callable[[], List[RELExample]]]): Optional callable that
+        reads a file containing task examples for few-shot learning. If None is
+        passed, then zero-shot learning will be used.
+    normalizer (Optional[Callable[[str], str]]): Optional normalizer function.
+    verbose (bool): Controls the verbosity of the task.
+    """
     labels_list = split_labels(labels)
     raw_examples = examples() if callable(examples) else examples
-    textcat_examples = (
-        [TextCatExample(**eg) for eg in raw_examples] if raw_examples else None
-    )
-    return TextCatTask(
+    rel_examples = [RELExample(**eg) for eg in raw_examples] if raw_examples else None
+    return RELTask(
         labels=labels_list,
         template=template,
         label_definitions=label_definitions,
-        examples=textcat_examples,
+        examples=rel_examples,
         normalizer=normalizer,
-        exclusive_classes=exclusive_classes,
-        allow_none=allow_none,
         verbose=verbose,
     )
 
 
-class TextCatTask:
+class RELTask(SerializableTask[RELExample]):
     def __init__(
         self,
-        labels: List[str],
-        template: str = _DEFAULT_TEXTCAT_TEMPLATE_V3,
+        labels: List[str] = [],
+        template: str = _DEFAULT_REL_TEMPLATE,
         label_definitions: Optional[Dict[str, str]] = None,
-        examples: Optional[List[TextCatExample]] = None,
+        examples: Optional[List[RELExample]] = None,
         normalizer: Optional[Callable[[str], str]] = None,
-        exclusive_classes: bool = False,
-        allow_none: bool = True,
         verbose: bool = False,
     ):
-        """Default TextCat task.
+        """Default REL task. Populates a `Doc._.rel` custom attribute.
 
-        You can use either binary or multilabel text classification based on the
-        labels you provide.
-
-        If a single label is provided, binary classification
-        will be used. The label will get a score of `0` or `1` in `doc.cats`.
-
-        If a comma-separated list of labels is provided, multilabel
-        classification will be used. The document labels in `doc.cats` will be a
-        dictionary of strings and their score.
-
-        Lastly, you can toggle between exclusive or no-exclusive text
-        categorization by passing a flag to the `exclusive_classes` parameter.
-
-        labels (str): Comma-separated list of labels to pass to the template. This task
-            assumes binary classification if a single label is provided.
+        labels (List[str]): List of labels to pass to the template.
+            Leave empty to populate it at initialization time (only if examples are provided).
         template (str): Prompt template passed to the model.
-        label_definitions (Optional[Dict[str, str]]): Optional dict mapping a label to a description of that label.
-            These descriptions are added to the prompt to help instruct the LLM on what to extract.
-        examples (Optional[Callable[[], Iterable[Any]]]): Optional callable that
+        label_definitions (Optional[Dict[str, str]]): Map of label -> description
+            of the label to help the language model output the entities wanted.
+            It is usually easier to provide these definitions rather than
+            full examples, although both can be provided.
+        examples (Optional[Callable[[], List[RELExample]]]): Optional callable that
             reads a file containing task examples for few-shot learning. If None is
             passed, then zero-shot learning will be used.
         normalizer (Optional[Callable[[str], str]]): Optional normalizer function.
-        exclusive_classes (bool): If True, require the language model to suggest only one
-            label per class. This is automatically set when using binary classification.
-        allow_none (bool): if True, there might be cases where no label is applicable.
-        verbose (bool): If True, show extra information.
+        verbose (bool): Controls the verbosity of the task.
         """
-        self._template = template
         self._normalizer = normalizer if normalizer else lowercase_normalizer()
         self._label_dict = {self._normalizer(label): label for label in labels}
+        self._template = template
         self._label_definitions = label_definitions
         self._examples = examples
-        # Textcat configuration
-        self._use_binary = True if len(self._label_dict) == 1 else False
-        self._exclusive_classes = exclusive_classes
-        self._allow_none = allow_none
         self._verbose = verbose
 
-        if self._use_binary and not self._exclusive_classes:
-            msg.warn(
-                "Binary classification should always be exclusive. Setting "
-                "the `exclusive_classes` parameter to True."
-            )
-            self._exclusive_classes = True
+    @classmethod
+    def _check_rel_extention(cls):
+        """Add `rel` extension if need be."""
+        if not Doc.has_extension("rel"):
+            Doc.set_extension("rel", default=[])
 
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
-                text=doc.text,
+                text=_preannotate(doc),
                 labels=list(self._label_dict.values()),
                 label_definitions=self._label_definitions,
                 examples=self._examples,
-                exclusive_classes=self._exclusive_classes,
-                allow_none=self._allow_none,
+                preannotate=_preannotate,
             )
             yield prompt
 
-    def _format_response(self, response: str) -> Dict[str, float]:
-        """Parse raw string response into a structured format
-
-        The returned dictionary contains the labels mapped to their score.
-        """
-        categories: Dict[str, float]
-        response = response.strip()
-        if self._use_binary:
-            # Binary classification: We only have one label
-            label: str = list(self._label_dict.values())[0]
-            score = 1.0 if response.upper() == "POS" else 0.0
-            categories = {label: score}
-        else:
-            # Multilabel classification
-            categories = {label: 0.0 for label in self._label_dict.values()}
-
-            pred_labels = response.split(",")
-            if self._exclusive_classes and len(pred_labels) > 1:
-                # Don't use anything but raise a debug message
-                # Don't raise an error. Let user abort if they want to.
-                msg.text(
-                    f"LLM returned multiple labels for this exclusive task: {pred_labels}.",
-                    " Will store an empty label instead.",
+    def _format_response(self, response: str) -> List[RelationItem]:
+        """Parse raw string response into a structured format"""
+        relations = []
+        for line in response.strip().split("\n"):
+            try:
+                relations.append(RelationItem.parse_raw(line))
+            except ValidationError:
+                msg.warn(
+                    "Validation issue",
+                    line,
                     show=self._verbose,
                 )
-                pred_labels = []
-
-            for pred in pred_labels:
-                if self._normalizer(pred.strip()) in self._label_dict:
-                    category = self._label_dict[self._normalizer(pred.strip())]
-                    categories[category] = 1.0
-        return categories
+        return relations
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[str]
     ) -> Iterable[Doc]:
+        self._check_rel_extention()
+
         for doc, prompt_response in zip(docs, responses):
-            cats = self._format_response(prompt_response)
-            doc.cats = cats
+            rels = self._format_response(prompt_response)
+            doc._.rel = rels
             yield doc
 
-    def scorer(
+    def initialize(
         self,
-        examples: Iterable[Example],
-    ) -> Dict[str, Any]:
-        return Scorer.score_cats(
-            examples,
-            attr="cats",
-            labels=self._label_dict.values(),
-            multi_label=not self._exclusive_classes,
-        )
+        get_examples: Callable[[], Iterable["Example"]],
+        nlp: Language,
+        labels: List[str] = [],
+    ) -> None:
+        """Initialize the SpanCat task, by auto-discovering labels.
+
+        Labels can be set through, by order of precedence:
+
+        - the `[initialize]` section of the pipeline configuration
+        - the `labels` argument supplied to the task factory
+        - the labels found in the examples
+
+        get_examples (Callable[[], Iterable["Example"]]): Callable that provides examples
+            for initialization.
+        nlp (Language): Language instance.
+        labels (List[str]): Optional list of labels.
+        """
+        self._check_rel_extention()
+
+        examples = get_examples()
+
+        if not labels:
+            labels = list(self._label_dict.values())
+
+        if not labels:
+            label_set = set()
+
+            for eg in examples:
+                rels: List[RelationItem] = eg.reference._.rel
+                for rel in rels:
+                    label_set.add(rel.relation)
+            labels = list(label_set)
+
+        self._label_dict = {self._normalizer(label): label for label in labels}
+
+    @property
+    def _cfg_keys(self) -> List[str]:
+        return [
+            "_label_dict",
+            "_template",
+            "_label_definitions",
+            "_verbose",
+        ]
+
+    @property
+    def _Example(self) -> Type[RELExample]:
+        return RELExample
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/util/parsing.py` & `spacy-llm-0.3.0/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tasks/util/span.py` & `spacy-llm-0.3.0/spacy_llm/tasks/util/span.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Callable, Dict, Iterable, List, Optional, Tuple
+from typing import Callable, Dict, Iterable, List, Optional, Tuple, Type
 
 import jinja2
 from spacy.tokens import Doc, Span
 
 from ...compat import Literal
 from ...registry import lowercase_normalizer
 from .examples import SpanExample
 from .parsing import find_substrings
+from .serialization import SerializableTask
 
 
-class SpanTask:
+class SpanTask(SerializableTask[SpanExample]):
     """Base class for Span-related tasks, eg NER and SpanCat."""
 
     def __init__(
         self,
         labels: List[str],
         template: str,
         label_definitions: Optional[Dict[str, str]] = {},
@@ -31,22 +32,14 @@
         self._label_definitions = label_definitions
         self._examples = examples
         self._validate_alignment(alignment_mode)
         self._alignment_mode = alignment_mode
         self._case_sensitive_matching = case_sensitive_matching
         self._single_match = single_match
 
-    def _validate_alignment(self, mode):
-        # ideally, this list should be taken from spaCy, but it's not currently exposed from doc.pyx.
-        alignment_modes = ("strict", "contract", "expand")
-        if mode not in alignment_modes:
-            raise ValueError(
-                f"Unsupported alignment mode '{mode}'. Supported modes: {', '.join(alignment_modes)}"
-            )
-
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
         environment = jinja2.Environment()
         _template = environment.from_string(self._template)
         for doc in docs:
             prompt = _template.render(
                 text=doc.text,
                 labels=list(self._label_dict.values()),
@@ -68,14 +61,26 @@
                 if norm_label in self._label_dict:
                     # Get the phrases / spans for each entity
                     if phrases.strip():
                         _phrases = [p.strip() for p in phrases.strip().split(",")]
                         output.append((self._label_dict[norm_label], _phrases))
         return output
 
+    @staticmethod
+    def _validate_alignment(alignment_mode: str):
+        """Raises error if specified alignment_mode is not supported.
+        alignment_mode (str): Alignment mode to check.
+        """
+        # ideally, this list should be taken from spaCy, but it's not currently exposed from doc.pyx.
+        alignment_modes = ("strict", "contract", "expand")
+        if alignment_mode not in alignment_modes:
+            raise ValueError(
+                f"Unsupported alignment mode '{alignment_mode}'. Supported modes: {', '.join(alignment_modes)}"
+            )
+
     def assign_spans(
         self,
         doc: Doc,
         spans: List[Span],
     ) -> None:
         """Assign spans to the document."""
         raise NotImplementedError()
@@ -99,7 +104,22 @@
                         start, end, alignment_mode=self._alignment_mode, label=label
                     )
                     if span is not None:
                         spans.append(span)
 
             self.assign_spans(doc, spans)
             yield doc
+
+    @property
+    def _cfg_keys(self) -> List[str]:
+        return [
+            "_label_dict",
+            "_template",
+            "_label_definitions",
+            "_alignment_mode",
+            "_case_sensitive_matching",
+            "_single_match",
+        ]
+
+    @property
+    def _Example(self) -> Type[SpanExample]:
+        return SpanExample
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/backends/test_dolly.py` & `spacy-llm-0.3.0/spacy_llm/tests/backends/test_openllama.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 import copy
 
-import spacy
 import pytest
+import spacy
 from confection import Config  # type: ignore[import]
 from thinc.compat import has_torch_cuda_gpu
 
 _PIPE_CFG = {
     "backend": {
-        "@llm_backends": "spacy.DollyHF.v1",
-        "model": "databricks/dolly-v2-3b",
+        "@llm_backends": "spacy.OpenLLaMa_HF.v1",
+        "model": "openlm-research/open_llama_3b_350bt_preview",
     },
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
 }
 
 _NLP_CONFIG = """
-
 [nlp]
 lang = "en"
 pipeline = ["llm"]
 batch_size = 128
 
 [components]
 
 [components.llm]
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
 
 [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1"
-model = "databricks/dolly-v2-3b"
+@llm_backends = spacy.OpenLLaMa_HF.v1
+model = "openlm-research/open_llama_3b_350bt_preview"
 """
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init():
-    """Test initialization and simple run"""
+    """Test initialization and simple run."""
     nlp = spacy.blank("en")
     nlp.add_pipe("llm", config=_PIPE_CFG)
     nlp("This is a test.")
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
+def test_init_with_set_config():
+    """Test initialization and simple run with changed config."""
+    nlp = spacy.blank("en")
+    cfg = copy.deepcopy(_PIPE_CFG)
+    cfg["backend"]["config_run"] = {"max_new_tokens": 32}
+    nlp.add_pipe("llm", config=cfg)
+    nlp("This is a test.")
+
+
+@pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_from_config():
     orig_config = Config().from_str(_NLP_CONFIG)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_invalid_model():
     orig_config = Config().from_str(_NLP_CONFIG)
     config = copy.deepcopy(orig_config)
-    config["components"]["llm"]["backend"]["model"] = "dolly-the-sheep"
+    config["components"]["llm"]["backend"]["model"] = "anything-else"
     with pytest.raises(ValueError, match="is not supported"):
         spacy.util.load_model_from_config(config, auto_fill=True)
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/backends/test_langchain.py` & `spacy-llm-0.3.0/spacy_llm/tests/backends/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/backends/test_minichain.py` & `spacy-llm-0.3.0/spacy_llm/tests/backends/test_minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/backends/test_rest.py` & `spacy-llm-0.3.0/spacy_llm/tests/backends/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.3.0/spacy_llm/tests/pipeline/test_llm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+import logging
+import sys
 import warnings
 from pathlib import Path
 from typing import Any, Dict, Iterable
 
 import pytest
 import spacy
 from spacy.language import Language
 from spacy.tokens import Doc
-
 from thinc.api import NumpyOps, get_current_ops
 
+import spacy_llm
+from spacy_llm.backends.rest.noop import _NOOP_RESPONSE
 from spacy_llm.pipeline import LLMWrapper
 from spacy_llm.registry import registry
 from spacy_llm.tasks import make_noop_task
+from spacy_llm.tasks.noop import _NOOP_PROMPT
 
-from ..compat import has_openai_key
 from ...cache import BatchCache
+from ..compat import has_openai_key
 
 
 @pytest.fixture
 def noop_config() -> Dict[str, Any]:
     """Returns NoOp config.
     RETURNS (Dict[str, Any]): NoOp config.
     """
     return {
+        "save_io": True,
         "task": {"@llm_tasks": "spacy.NoOp.v1"},
         "backend": {"api": "NoOp", "config": {"model": "NoOp"}},
     }
 
 
 @pytest.fixture
 def nlp(noop_config) -> Language:
@@ -47,14 +52,20 @@
     if not isinstance(ops, NumpyOps) and n_process != 1:
         pytest.skip("Only test multiple processes on CPU")
     docs = list(
         nlp.pipe(texts=["This is a test", "This is another test"], n_process=n_process)
     )
     assert len(docs) == 2
 
+    for doc in docs:
+        llm_io = doc.user_data["llm_io"]
+
+        assert llm_io["llm"]["prompt"] == _NOOP_PROMPT
+        assert llm_io["llm"]["response"] == _NOOP_RESPONSE
+
 
 @pytest.mark.parametrize("n_process", [1, 2])
 def test_llm_pipe_with_cache(tmp_path: Path, n_process: int):
     """Test call .pipe() with pre-cached docs"""
     ops = get_current_ops()
     if not isinstance(ops, NumpyOps) and n_process != 1:
         pytest.skip("Only test multiple processes on CPU")
@@ -90,24 +101,26 @@
     """Test call .pipe() with empty batch."""
     assert list(nlp.pipe(texts=[])) == []
 
 
 def test_llm_serialize_bytes():
     llm = LLMWrapper(
         task=make_noop_task(),
+        save_io=False,
         backend=None,  # type: ignore
         cache=BatchCache(path=None, batch_size=0, max_batches_in_mem=0),
         vocab=None,  # type: ignore
     )
     llm.from_bytes(llm.to_bytes())
 
 
 def test_llm_serialize_disk():
     llm = LLMWrapper(
         task=make_noop_task(),
+        save_io=False,
         backend=None,  # type: ignore
         cache=BatchCache(path=None, batch_size=0, max_batches_in_mem=0),
         vocab=None,  # type: ignore
     )
 
     with spacy.util.make_tempdir() as tmp_dir:
         llm.to_disk(tmp_dir / "llm")
@@ -152,7 +165,63 @@
         "expected by `backend` (`typing.Iterable[str]`)."
     )
     assert (
         str(record[1].message)
         == "Type returned from `backend` (`typing.Iterable[str]`) doesn't match type "
         "expected by `task.parse_responses()` (`typing.Iterable[float]`)."
     )
+
+
+@pytest.mark.parametrize("use_pipe", [True, False])
+def test_llm_logs_at_debug_level(
+    nlp: Language, use_pipe: bool, caplog: pytest.LogCaptureFixture
+):
+    with caplog.at_level(logging.INFO):
+        if use_pipe:
+            doc = next(nlp.pipe(["This is a test"]))
+        else:
+            doc = nlp("This is a test")
+
+    assert "spacy_llm" not in caplog.text
+    assert doc.text not in caplog.text
+
+    with caplog.at_level(logging.DEBUG):
+        if use_pipe:
+            doc = next(nlp.pipe(["This is a test"]))
+        else:
+            doc = nlp("This is a test")
+
+    assert "spacy_llm" in caplog.text
+    assert doc.text in caplog.text
+
+    assert f"Generated prompt for doc: {doc.text}" in caplog.text
+    assert "Don't do anything" in caplog.text
+    assert f"LLM response for doc: {doc.text}" in caplog.text
+
+
+def test_llm_logs_default_null_handler(nlp: Language, capsys: pytest.CaptureFixture):
+
+    doc = nlp("This is a test")
+
+    captured = capsys.readouterr()
+    assert captured.out == ""
+    assert captured.err == ""
+
+    # Add a basic Stream Handler
+    stream_handler = logging.StreamHandler(sys.stdout)
+    spacy_llm.logger.addHandler(stream_handler)
+    spacy_llm.logger.setLevel(logging.DEBUG)
+
+    doc = nlp("This is a test")
+    captured = capsys.readouterr()
+    assert f"Generated prompt for doc: {doc.text}" in captured.out
+    assert "Don't do anything" in captured.out
+    assert f"LLM response for doc: {doc.text}" in captured.out
+
+    # Remove the Stream Handler from the spacy_llm logger
+    spacy_llm.logger.removeHandler(stream_handler)
+
+    doc = nlp("This is a test with no handler")
+    captured = capsys.readouterr()
+    assert f"Generated prompt for doc: {doc.text}" not in captured.out
+    assert "Don't do anything" not in captured.out
+    assert f"LLM response for doc: {doc.text}" not in captured.out
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/tasks/examples/rel_examples.jsonl` & `spacy-llm-0.3.0/spacy_llm/tests/tasks/examples/rel_examples.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.3.0/spacy_llm/tests/tasks/test_ner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,22 @@
+import json
 from pathlib import Path
-from typing import Iterable
 
 import pytest
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
 from spacy.tokens import Span
 from spacy.training import Example
 from spacy.util import make_tempdir
 
-from spacy_llm.registry import (
-    fewshot_reader,
-    file_reader,
-    lowercase_normalizer,
-    registry,
-    strip_normalizer,
-)
-from spacy_llm.tasks.ner import make_ner_task_v2
+from spacy_llm.registry import fewshot_reader, file_reader, lowercase_normalizer
+from spacy_llm.registry import strip_normalizer
+from spacy_llm.tasks.ner import NERTask, make_ner_task_v2
 from spacy_llm.tasks.util import find_substrings
 from spacy_llm.util import assemble_from_config
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 TEMPLATES_DIR = Path(__file__).parent / "templates"
@@ -672,26 +667,44 @@
 LOC
 
 Here is the text: Alice and Bob went to the supermarket
 """.strip()
     )
 
 
-@pytest.mark.parametrize("n_detections", [0, 1, 2])
-def test_ner_scoring(zeroshot_cfg_string, n_detections):
-    @registry.llm_backends("Dummy")
-    def factory():
-        def b(prompts: Iterable[str]) -> Iterable[str]:
-            for _ in prompts:
-                yield ("PER: Alice,Bob")
+@pytest.fixture
+def noop_config():
+    return """
+    [nlp]
+    lang = "en"
+    pipeline = ["llm"]
+    batch_size = 128
 
-        return b
+    [components]
 
-    config = Config().from_str(zeroshot_cfg_string)
-    config["components"]["llm"]["backend"] = {"@llm_backends": "Dummy"}
+    [components.llm]
+    factory = "llm"
+
+    [components.llm.task]
+    @llm_tasks = "spacy.NER.v2"
+    labels = PER,ORG,LOC
+
+    [components.llm.task.normalizer]
+    @misc = "spacy.LowercaseNormalizer.v1"
+
+    [components.llm.backend]
+    @llm_backends = "test.NoOpBackend.v1"
+    output = "PER: Alice,Bob"
+    """
+
+
+@pytest.mark.parametrize("n_detections", [0, 1, 2])
+def test_ner_scoring(noop_config, n_detections):
+
+    config = Config().from_str(noop_config)
     nlp = assemble_from_config(config)
 
     examples = []
 
     for text in ["Alice works with Bob.", "Bob lives with Alice."]:
         predicted = nlp.make_doc(text)
         reference = predicted.copy()
@@ -702,7 +715,97 @@
         ][:n_detections]
 
         examples.append(Example(predicted, reference))
 
     scores = nlp.evaluate(examples)
 
     assert scores["ents_p"] == n_detections / 2
+
+
+def test_ner_init(noop_config):
+
+    config = Config().from_str(noop_config)
+    del config["components"]["llm"]["task"]["labels"]
+    nlp = assemble_from_config(config)
+
+    examples = []
+
+    for text in [
+        "Alice works with Bob in London.",
+        "Bob lives with Alice in Manchester.",
+    ]:
+        predicted = nlp.make_doc(text)
+        reference = predicted.copy()
+
+        reference.ents = [
+            Span(reference, 0, 1, label="PER"),
+            Span(reference, 3, 4, label="PER"),
+            Span(reference, 5, 6, label="LOC"),
+        ]
+
+        examples.append(Example(predicted, reference))
+
+    _, llm = nlp.pipeline[0]
+    task: NERTask = llm._task
+
+    assert set(task._label_dict.values()) == set()
+    nlp.initialize(lambda: examples)
+    assert set(task._label_dict.values()) == {"PER", "LOC"}
+
+
+def test_ner_serde(noop_config):
+
+    config = Config().from_str(noop_config)
+    del config["components"]["llm"]["task"]["labels"]
+
+    nlp1 = assemble_from_config(config)
+    nlp2 = assemble_from_config(config)
+
+    labels = {"loc": "LOC", "per": "PER"}
+
+    task1: NERTask = nlp1.get_pipe("llm")._task
+    task2: NERTask = nlp2.get_pipe("llm")._task
+
+    # Artificially add labels to task1
+    task1._label_dict = labels
+
+    assert task1._label_dict == labels
+    assert task2._label_dict == dict()
+
+    b = nlp1.to_bytes()
+    nlp2.from_bytes(b)
+
+    assert task1._label_dict == task2._label_dict == labels
+
+
+def test_ner_to_disk(noop_config, tmp_path: Path):
+
+    config = Config().from_str(noop_config)
+    del config["components"]["llm"]["task"]["labels"]
+
+    nlp1 = assemble_from_config(config)
+    nlp2 = assemble_from_config(config)
+
+    labels = {"loc": "LOC", "per": "PER"}
+
+    task1: NERTask = nlp1.get_pipe("llm")._task
+    task2: NERTask = nlp2.get_pipe("llm")._task
+
+    # Artificially add labels to task1
+    task1._label_dict = labels
+
+    assert task1._label_dict == labels
+    assert task2._label_dict == dict()
+
+    path = tmp_path / "model"
+
+    nlp1.to_disk(path)
+
+    cfgs = list(path.rglob("cfg"))
+    assert len(cfgs) == 1
+
+    cfg = json.loads(cfgs[0].read_text())
+    assert cfg["_label_dict"] == labels
+
+    nlp2.from_disk(path)
+
+    assert task1._label_dict == task2._label_dict == labels
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/tasks/test_spancat.py` & `spacy-llm-0.3.0/spacy_llm/tests/tasks/test_spancat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from pathlib import Path
-from typing import Iterable
 
 import pytest
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
 from spacy.tokens import Span
 from spacy.training import Example
 from spacy.util import make_tempdir
 
-from spacy_llm.registry import (
-    fewshot_reader,
-    lowercase_normalizer,
-    registry,
-    strip_normalizer,
-)
+from spacy_llm.registry import fewshot_reader, lowercase_normalizer, strip_normalizer
 from spacy_llm.tasks import make_spancat_task_v2
+from spacy_llm.tasks.spancat import SpanCatTask
 from spacy_llm.tasks.util import find_substrings
 from spacy_llm.util import assemble_from_config
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 
@@ -479,26 +474,44 @@
 
         with pytest.raises(ValidationError):
             make_spancat_task_v2(
                 labels="PER,ORG,LOC", examples=fewshot_reader(tmp_path)
             )
 
 
-@pytest.mark.parametrize("n_detections", [0, 1, 2])
-def test_spancat_scoring(zeroshot_cfg_string, n_detections):
-    @registry.llm_backends("Dummy")
-    def factory():
-        def b(prompts: Iterable[str]) -> Iterable[str]:
-            for _ in prompts:
-                yield ("PER: Alice,Bob")
+@pytest.fixture
+def noop_config():
+    return """
+    [nlp]
+    lang = "en"
+    pipeline = ["llm"]
+    batch_size = 128
+
+    [components]
+
+    [components.llm]
+    factory = "llm"
 
-        return b
+    [components.llm.task]
+    @llm_tasks = "spacy.SpanCat.v2"
+    labels = ["PER", "ORG", "LOC"]
 
-    config = Config().from_str(zeroshot_cfg_string)
-    config["components"]["llm"]["backend"] = {"@llm_backends": "Dummy"}
+    [components.llm.task.normalizer]
+    @misc = "spacy.LowercaseNormalizer.v1"
+
+    [components.llm.backend]
+    @llm_backends = "test.NoOpBackend.v1"
+    output = "PER: Bob,Alice"
+    """
+
+
+@pytest.mark.parametrize("n_detections", [0, 1, 2])
+def test_spancat_scoring(noop_config, n_detections):
+
+    config = Config().from_str(noop_config)
     nlp = assemble_from_config(config)
 
     examples = []
 
     for text in ["Alice works with Bob.", "Bob lives with Alice."]:
         predicted = nlp.make_doc(text)
         reference = predicted.copy()
@@ -509,7 +522,63 @@
         ][:n_detections]
 
         examples.append(Example(predicted, reference))
 
     scores = nlp.evaluate(examples)
 
     assert scores["spans_sc_p"] == n_detections / 2
+
+
+def test_spancat_init(noop_config):
+
+    config = Config().from_str(noop_config)
+    del config["components"]["llm"]["task"]["labels"]
+    nlp = assemble_from_config(config)
+
+    examples = []
+
+    for text in [
+        "Alice works with Bob in London.",
+        "Bob lives with Alice in Manchester.",
+    ]:
+        predicted = nlp.make_doc(text)
+        reference = predicted.copy()
+
+        reference.spans["sc"] = [
+            Span(reference, 0, 1, label="PER"),
+            Span(reference, 3, 4, label="PER"),
+            Span(reference, 5, 6, label="LOC"),
+        ]
+
+        examples.append(Example(predicted, reference))
+
+    _, llm = nlp.pipeline[0]
+    task: SpanCatTask = llm._task
+
+    assert set(task._label_dict.values()) == set()
+    nlp.initialize(lambda: examples)
+    assert set(task._label_dict.values()) == {"PER", "LOC"}
+
+
+def test_spancat_serde(noop_config):
+
+    config = Config().from_str(noop_config)
+    del config["components"]["llm"]["task"]["labels"]
+
+    nlp1 = assemble_from_config(config)
+    nlp2 = assemble_from_config(config)
+
+    labels = {"loc": "LOC", "per": "PER"}
+
+    task1: SpanCatTask = nlp1.get_pipe("llm")._task
+    task2: SpanCatTask = nlp2.get_pipe("llm")._task
+
+    # Artificially add labels to task1
+    task1._label_dict = labels
+
+    assert task1._label_dict == labels
+    assert task2._label_dict == dict()
+
+    b = nlp1.to_bytes()
+    nlp2.from_bytes(b)
+
+    assert task1._label_dict == task2._label_dict == labels
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.3.0/spacy_llm/tests/tasks/test_textcat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,22 @@
+import json
 from pathlib import Path
 from typing import Iterable
 
 import pytest
 import spacy
 import srsly
 from confection import Config
 from pydantic import ValidationError
 from spacy.training import Example
 from spacy.util import make_tempdir
 
-from spacy_llm.registry import (
-    fewshot_reader,
-    file_reader,
-    lowercase_normalizer,
-    registry,
-)
-from spacy_llm.tasks.textcat import make_textcat_task_v3
+from spacy_llm.registry import fewshot_reader, file_reader, lowercase_normalizer
+from spacy_llm.registry import registry
+from spacy_llm.tasks.textcat import TextCatTask, make_textcat_task_v3
 from spacy_llm.util import assemble_from_config
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 TEMPLATES_DIR = Path(__file__).parent / "templates"
 
@@ -703,7 +700,107 @@
 
 
 Text:
 '''
 You need to increase the temperature when baking, it looks undercooked.
 '''""".strip()
     )
+
+
+@pytest.fixture
+def noop_config():
+    return """
+    [nlp]
+    lang = "en"
+    pipeline = ["llm"]
+    batch_size = 128
+
+    [components]
+
+    [components.llm]
+    factory = "llm"
+
+    [components.llm.task]
+    @llm_tasks = "spacy.TextCat.v1"
+
+    [components.llm.task.normalizer]
+    @misc = "spacy.LowercaseNormalizer.v1"
+
+    [components.llm.backend]
+    @llm_backends = "test.NoOpBackend.v1"
+    """
+
+
+@pytest.mark.parametrize("init_from_config", [True, False])
+def test_textcat_init(noop_config, init_from_config: bool):
+
+    config = Config().from_str(noop_config)
+    if init_from_config:
+        config["initialize"] = {"components": {"llm": {"labels": ["Test"]}}}
+    nlp = assemble_from_config(config)
+
+    examples = []
+
+    for i, text in enumerate(INSULTS):
+        predicted = nlp.make_doc(text)
+        reference = predicted.copy()
+
+        if i < (len(INSULTS) // 2):
+            reference.cats = {"Insult": 1.0, "Compliment": 0.0}
+        else:
+            reference.cats = {"Insult": 0.0, "Compliment": 1.0}
+
+        examples.append(Example(predicted, reference))
+
+    _, llm = nlp.pipeline[0]
+    task: TextCatTask = llm._task
+
+    if init_from_config:
+        target = {"Test"}
+    else:
+        target = set()
+    assert set(task._label_dict.values()) == target
+
+    nlp.initialize(lambda: examples)
+
+    if init_from_config:
+        target = {"Test"}
+    else:
+        target = {"Insult", "Compliment"}
+    assert set(task._label_dict.values()) == target
+
+
+def test_textcat_serde(noop_config, tmp_path: Path):
+
+    config = Config().from_str(noop_config)
+
+    nlp1 = assemble_from_config(config)
+    nlp2 = assemble_from_config(config)
+    nlp3 = assemble_from_config(config)
+
+    labels = {"insult": "INSULT", "compliment": "COMPLIMENT"}
+
+    task1: TextCatTask = nlp1.get_pipe("llm")._task
+    task2: TextCatTask = nlp2.get_pipe("llm")._task
+    task3: TextCatTask = nlp3.get_pipe("llm")._task
+
+    # Artificially add labels to task1
+    task1._label_dict = labels
+
+    assert task1._label_dict == labels
+    assert task2._label_dict == dict()
+    assert task3._label_dict == dict()
+
+    path = tmp_path / "model"
+
+    nlp1.to_disk(path)
+
+    cfgs = list(path.rglob("cfg"))
+    assert len(cfgs) == 1
+
+    cfg = json.loads(cfgs[0].read_text())
+    assert cfg["_label_dict"] == labels
+
+    nlp2.from_disk(path)
+    nlp3.from_bytes(nlp1.to_bytes())
+
+    assert task1._label_dict == task2._label_dict == task3._label_dict == labels
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/test_cache.py` & `spacy-llm-0.3.0/spacy_llm/tests/test_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+import copy
 import time
 from pathlib import Path
 from typing import Dict
 
 import pytest
-import srsly  # type: ignore[import]
 import spacy
-from spacy import Language
+import srsly  # type: ignore[import]
+from spacy.language import Language
 from spacy.tokens import DocBin
-import copy
 
 from ..cache import BatchCache
 
-
 _DEFAULT_CFG = {
     "backend": {"api": "NoOp", "config": {"model": "NoOp"}},
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
     "cache": {
         "batch_size": 2,
         "max_batches_in_mem": 3,
     },
```

### Comparing `spacy-llm-0.2.1/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.3.0/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/spacy_llm/ty.py` & `spacy-llm-0.3.0/spacy_llm/ty.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,74 @@
 import inspect
 import typing
 import warnings
-from typing import Any, Callable, Dict, Iterable, Optional, Union, Type, List
+from pathlib import Path
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, Union
+from typing import cast
 
 from spacy.tokens import Doc
+from spacy.training.example import Example
 from spacy.vocab import Vocab
 
 from .backends import integration
 from .compat import Protocol, runtime_checkable
 
-
 _Prompt = Any
 _Response = Any
 
 PromptExecutor = Callable[[Iterable[_Prompt]], Iterable[_Response]]
 ExamplesConfigType = Union[
     Iterable[Dict[str, Any]], Callable[[], Iterable[Dict[str, Any]]], None
 ]
 
 
 @runtime_checkable
+class Serializable(Protocol):
+    def to_bytes(
+        self,
+        *,
+        exclude: Tuple[str] = cast(Tuple[str], tuple()),
+    ) -> bytes:
+        ...
+
+    def from_bytes(
+        self,
+        bytes_data: bytes,
+        *,
+        exclude: Tuple[str] = cast(Tuple[str], tuple()),
+    ) -> bytes:
+        ...
+
+    def to_disk(
+        self,
+        path: Path,
+        *,
+        exclude: Tuple[str] = cast(Tuple[str], tuple()),
+    ) -> bytes:
+        ...
+
+    def from_disk(
+        self,
+        path: Path,
+        *,
+        exclude: Tuple[str] = cast(Tuple[str], tuple()),
+    ):
+        ...
+
+
+@runtime_checkable
+class Scorable(Protocol):
+    def scorer(
+        self,
+        examples: Iterable[Example],
+    ) -> Dict[str, Any]:
+        """Scores performance on examples."""
+
+
+@runtime_checkable
 class LLMTask(Protocol):
     def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[_Prompt]:
         ...
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[_Response]
     ) -> Iterable[Doc]:
@@ -96,31 +141,31 @@
         return typing.get_type_hints(backend)
 
     if not hasattr(backend, "__call__"):
         raise ValueError("The object supplied as backend must implement `__call__()`.")
 
     # Assume that __call__() has the necessary type info - except in the case of integration.Backend, for which
     # we know this is not the case.
-    if not isinstance(backend, integration.Backend):
+    if not isinstance(backend, integration.RemoteBackend):
         return typing.get_type_hints(backend.__call__)
 
-    # If this is an instance of integrations.Backend: read type information from .query() instead, only keep
+    # If this is an instance of integrations.RemoteBackend: read type information from .query() instead, only keep
     # information on Iterable args.
     signature = typing.get_type_hints(backend.query).items()
     to_ignore: List[str] = []
     for k, v in signature:
         if not (hasattr(v, "__origin__") and issubclass(v.__origin__, Iterable)):
             to_ignore.append(k)
 
     signature = {
         k: v
         for k, v in typing.get_type_hints(backend.query).items()
         # In Python 3.8+ (or 3.6+ if typing_utils is installed) the check for the origin class should be done using
         # typing.get_origin().
-        if hasattr(v, "__origin__") and issubclass(v.__origin__, Iterable)
+        if k not in to_ignore
     }
     assert len(signature) == 2
     assert "return" in signature
     return signature
 
 
 def validate_types(task: LLMTask, backend: PromptExecutor) -> None:
```

### Comparing `spacy-llm-0.2.1/spacy_llm/util.py` & `spacy-llm-0.3.0/spacy_llm/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from typing import Any, Dict, Iterable, List, Union
 from pathlib import Path
+from typing import Any, Dict, Iterable, List, Union
 
 from confection import Config
 from spacy.language import Language
 from spacy.util import SimpleFrozenDict, get_sourced_components, load_config
 from spacy.util import load_model_from_config
 
 
 def split_labels(labels: Union[str, Iterable[str]]) -> List[str]:
     """Split a comma-separated list of labels.
     If input is a list already, just strip each entry of the list
 
     labels (Union[str, Iterable[str]]): comma-separated string or list of labels
     RETURNS (List[str]): a split and stripped list of labels
     """
+    if not labels:
+        return []
     labels = labels.split(",") if isinstance(labels, str) else labels
     return [label.strip() for label in labels]
 
 
 def assemble_from_config(config: Config) -> Language:
     """Assemble a spaCy pipeline from a confection Config object.
```

### Comparing `spacy-llm-0.2.1/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: spacy-llm
-Version: 0.2.1
-Summary: Integrating LLMs into structured NLP pipelines
-Author: Explosion
-Author-email: contact@explosion.ai
-License: MIT
-Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
-Project-URL: Source, https://github.com/explosion/spacy-llm
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: minichain
-Provides-Extra: langchain
-Provides-Extra: transformers
-License-File: LICENSE
-
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # spacy-llm: Integrating LLMs into structured NLP pipelines
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/explosion/spacy-llm/actions/workflows/test.yml)
 [![pypi Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
@@ -134,15 +102,15 @@
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NER.v2"
 labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
 [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1"
+@llm_backends = "spacy.Dolly_HF.v1"
 # For better performance, use databricks/dolly-v2-12b instead
 model = "databricks/dolly-v2-3b"
 ```
 
 Now run:
 
 ```python
@@ -230,26 +198,105 @@
 # config.cfg (excerpt)
 [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1"
 labels = LABEL1,LABEL2,LABEL3
 my_other_config_val = 0.3
 ```
 
+## Logging
+
+spacy-llm has a built-in logger that can log the prompt sent to the LLM as well as its raw response. This logger uses the debug level and by default has a `logging.NullHandler()` configured.
+
+In order to use this logger, you can setup a simple handler like this:
+
+```python
+import logging
+import spacy_llm
+
+
+spacy_llm.logger.addHandler(logging.StreamHandler())
+spacy_llm.logger.setLevel(logging.DEBUG)
+```
+
+> NOTE: Any `logging` handler will work here so you probably want to use some sort of rotating `FileHandler` as the generated prompts can be quite long, especially for tasks with few-shot examples.
+
+
+Then when using the pipeline you'll be able to view the prompt and response.
+
+E.g. with the config and code from [Example 1](##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
+
+
+```python
+from spacy_llm.util import assemble
+
+
+nlp = assemble("config.cfg")
+doc = nlp("You look gorgeous!")
+print(doc.cats)
+```
+
+You will see `logging` output similar to:
+
+```
+Generated prompt for doc: You look gorgeous!
+
+You are an expert Text Classification system. Your task is to accept Text as input
+and provide a category for the text based on the predefined labels.
+
+Classify the text below to any of the following labels: COMPLIMENT, INSULT
+The task is non-exclusive, so you can provide more than one label as long as
+they're comma-delimited. For example: Label1, Label2, Label3.
+Do not put any other text in your answer, only one or more of the provided labels with nothing before or after.
+If the text cannot be classified into any of the provided labels, answer `==NONE==`.
+
+Here is the text that needs classification
+
+
+Text:
+'''
+You look gorgeous!
+'''
+
+Backend response for doc: You look gorgeous!
+COMPLIMENT
+```
+
+`print(doc.cats)` to standard output should look like:
+
+```
+{'COMPLIMENT': 1.0, 'INSULT': 0.0}
+```
+
 ## 📓 API
 
-Each `llm` component is defined by two main settings:
+`spacy-llm` exposes a `llm` factory that accepts the following configuration options:
+
+| Argument  | Type                                        | Description                                                                         |
+| --------- | ------------------------------------------- | ----------------------------------------------------------------------------------- |
+| `task`    | `Optional[LLMTask]`                         | An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks).        |
+| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a specific LLM API. See [docs](#backends).                        |
+| `cache`   | `Cache`                                     | Cache to use for caching prompts and responses per doc (batch). See [docs](#cache). |
+| `save_io` | `bool`                                      | Whether to save prompts/responses within `Doc.user_data["llm_io"]`                  |
+
+An `llm` component is defined by two main settings:
 
 - A [**task**](#tasks), defining the prompt to send to the LLM as well as the functionality to parse the resulting response
   back into structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects.
 - A [**backend**](#backends) defining the model to use and how to connect to it. Note that `spacy-llm` supports both access to external
   APIs (such as OpenAI) as well as access to self-hosted open-source LLMs (such as using Dolly through Hugging Face).
 
-Moreover, the component also implements [**caching**](#cache) functionality to avoid running
+Moreover, `spacy-llm` exposes a customizable [**caching**](#cache) functionality to avoid running
 the same document through an LLM service (be it local or through a REST API) more than once.
 
+Finally, you can choose to save a stringified version of LLM prompts/responses
+within the `Doc.user_data["llm_io"]` attribute by setting `save_io` to `True`.
+`Doc.user_data["llm_io"]` is a dictionary containing one entry for every LLM component
+within the spaCy pipeline. Each entry is itself a dictionary, with two keys:
+`prompt` and `response`.
+
 ### Tasks
 
 A _task_ defines an NLP problem or question, that will be sent to the LLM via a prompt. Further, the task defines
 how to parse the LLM's responses back into structured information. All tasks are registered in spaCy's `llm_tasks` registry.
 
 Practically speaking, a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py).
 It needs to define a `generate_prompts` function and a `parse_responses` function.
@@ -371,15 +418,14 @@
 | `labels`                  | `str`                                   |              | Comma-separated list of labels.                                                                                                              |
 | `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`       | Optional function that generates examples for few-shot learning.                                                                             |
 | `normalizer`              | `Optional[Callable[[str], str]]`        | `None`       | Function that normalizes the labels as returned by the LLM. If `None`, defaults to `spacy.LowercaseNormalizer.v1`.                           |
 | `alignment_mode`          | `str`                                   | `"contract"` | Alignment mode in case the LLM returns entities that do not align with token boundaries. Options are `"strict"`, `"contract"` or `"expand"`. |
 | `case_sensitive_matching` | `bool`                                  | `False`      | Whether to search without case sensitivity.                                                                                                  |
 | `single_match`            | `bool`                                  | `False`      | Whether to match an entity in the LLM's response only once (the first hit) or multiple times.                                                |
 
-
 The NER task implementation doesn't currently ask the LLM for specific offsets, but simply expects a list of strings that represent the enties in the document.
 This means that a form of string matching is required. This can be configured by the following parameters:
 
 - The `single_match` parameter is typically set to `False` to allow for multiple matches. For instance, the response from the LLM might only mention the entity "Paris" once, but you'd still
   want to mark it every time it occurs in the document.
 - The case-sensitive matching is typically set to `False` to be robust against case variances in the LLM's output.
 - The `alignment_mode` argument is used to match entities as returned by the LLM to the tokens from the original `Doc` - specifically it's used as argument
@@ -595,14 +641,79 @@
 @llm_tasks = "spacy.REL.v1"
 labels = ["LivesIn", "Visits"]
 [components.llm.task.examples]
 @misc = "spacy.FewShotReader.v1"
 path = "rel_examples.jsonl"
 ```
 
+#### spacy.Lemma.v1
+
+The `Lemma.v1` task lemmatizes the provided text and updates the `lemma_` attribute in the doc's tokens accordingly.
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Lemma.v1"
+examples = null
+```
+
+| Argument                  | Type                                    | Default                                                   | Description                                                                                                                                           |
+| ------------------------- | --------------------------------------- |-----------------------------------------------------------| ----------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `template`                | `str`                                   | [lemma.jinja](./spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM backend. Default templates for each task are located in the `spacy_llm/tasks/templates` directory.              |
+| `examples`                | `Optional[Callable[[], Iterable[Any]]]` | `None`                                                    | Optional function that generates examples for few-shot learning.                                                                                      |
+
+`Lemma.v1` prompts the LLM to lemmatize the passed text and return the lemmatized version as a list of tokens and their
+corresponding lemma. E. g. the text 
+`I'm buying ice cream for my friends` should invoke the response
+```
+I: I
+'m: be
+buying: buy
+ice: ice
+cream: cream
+for: for
+my: my
+friends: friend
+.: .
+```
+
+If for any given text/doc instance the number of lemmas returned by the LLM doesn't match the number of tokens recognized 
+by spaCy, no lemmas are stored in the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is updated with
+the lemma suggested by the LLM.
+
+To perform few-shot learning, you can write down a few examples in a separate file, and provide these to be injected into the prompt to the LLM.
+The default reader `spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+
+```yaml
+- text: I'm buying ice cream.
+  lemmas:
+    - "I": "I"
+    - "'m": "be"
+    - "buying": "buy"
+    - "ice": "ice"
+    - "cream": "cream"
+    - ".": "."
+
+- text: I've watered the plants.
+  lemmas: 
+    - "I": "I"
+    - "'ve": "have"
+    - "watered": "water"
+    - "the": "the"
+    - "plants": "plant"
+    - ".": "."
+```
+
+```ini
+[components.llm.task]
+@llm_tasks = "spacy.Lemma.v1"
+[components.llm.task.examples]
+@misc = "spacy.FewShotReader.v1"
+path = "lemma_examples.yml"
+```
+
 #### spacy.NoOp.v1
 
 This task is only useful for testing - it tells the LLM to do nothing, and does not set any fields on the `docs`.
 
 ```ini
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
@@ -740,56 +851,145 @@
 | -------- | ------------------------------------------------------------------------------ | ------- | ------------------------------------------------------------------------------------ |
 | `api`    | `str`                                                                          |         | The name of an API supported by LangChain, e.g. "OpenAI".                            |
 | `config` | `Dict[Any, Any]`                                                               | `{}`    | Further configuration passed on to the backend.                                      |
 | `query`  | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None`  | Function that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
 
 The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for each given textual prompt.
 
-#### spacy.DollyHF.v1
+#### spacy.Dolly_HF.v1
 
 To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
 This allows you to have the setting `device=cuda:0` in your config, which ensures that the model is loaded entirely on the GPU (and fails otherwise).
 
+You can do so with
+
 ```shell
-python -m pip install "torch>=1.13.1,<2.0"
-python -m pip install "transformers>=4.28.1,<5.0"
-# Or install with spacy-llm directly
-python -m pip install "spacy-llm[transformers]"
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ```
 
 If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
 which may ultimately result in extremely slow queries.
 
 ```shell
 python -m pip install "accelerate>=0.16.0,<1.0"
 ```
 
 Example config block:
 
 ```ini
 [components.llm.backend]
-@llm_backends = "spacy.DollyHF.v1"
+@llm_backends = "spacy.Dolly_HF.v1"
 model = "databricks/dolly-v2-3b"
 ```
 
-| Argument | Type             | Default | Description                                                                                      |
-| -------- | ---------------- | ------- | ------------------------------------------------------------------------------------------------ |
-| `model`  | `str`            |         | The name of a Dolly model that is supported.                                                     |
-| `config` | `Dict[Any, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
+| Argument      | Type             | Default | Description                                                                                      |
+| ------------- | ---------------- | ------- | ------------------------------------------------------------------------------------------------ |
+| `model`       | `str`            |         | The name of a Dolly model that is supported.                                                     |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.pipeline()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                               |
 
 Supported models (see the [Databricks models page](https://huggingface.co/databricks) on Hugging Face for details):
 
 - `"databricks/dolly-v2-3b"`
 - `"databricks/dolly-v2-7b"`
 - `"databricks/dolly-v2-12b"`
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
 
+#### spacy.StableLM_HF.v1
+
+To use this backend, ideally you have a GPU enabled and have installed `transformers`, `torch` and CUDA in your virtual environment.
+
+You can do so with
+
+```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
+```
+
+If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries.
+
+```shell
+python -m pip install "accelerate>=0.16.0,<1.0"
+```
+
+Example config block:
+
+```ini
+[components.llm.backend]
+@llm_backends = "spacy.StableLM_HF.v1"
+model = "stabilityai/stablelm-tuned-alpha-7b"
+```
+
+| Argument      | Type             | Default | Description                                                                                                                  |
+| ------------- | ---------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `model`       | `str`            |         | The name of a StableLM model that is supported.                                                                              |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                                                           |
+
+Supported models (see the [Stability AI StableLM GitHub repo](https://github.com/Stability-AI/StableLM/#stablelm-alpha) for details):
+
+- `"stabilityai/stablelm-base-alpha-3b"`
+- `"stabilityai/stablelm-base-alpha-7b"`
+- `"stabilityai/stablelm-tuned-alpha-3b"`
+- `"stabilityai/stablelm-tuned-alpha-7b"`
+
+Note that Hugging Face will download this model the first time you use it - you can
+[define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
+by setting the environmental variable `HF_HOME`.
+
+#### spacy.OpenLLaMaHF.v1
+
+To use this backend, ideally you have a GPU enabled and have installed
+
+- `transformers[sentencepiece]`
+- `torch`
+- CUDA
+  in your virtual environment.
+
+You can do so with
+
+```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
+```
+
+If you don't have access to a GPU, you can install `accelerate` and set`device_map=auto` instead, but be aware that this may result in some layers getting distributed to the CPU or even the hard drive,
+which may ultimately result in extremely slow queries.
+
+```shell
+python -m pip install "accelerate>=0.16.0,<1.0"
+```
+
+Example config block:
+
+```ini
+[components.llm.backend]
+@llm_backends = "spacy.OpenLLaMaHF.v1"
+model = "openlm-research/open_llama_3b_350bt_preview"
+```
+
+| Argument      | Type             | Default | Description                                                                                                                  |
+| ------------- | ---------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `model`       | `str`            |         | The name of a OpenLLaMa model that is supported.                                                                             |
+| `config_init` | `Dict[str, Any]` | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]` | `{}`    | Further configuration used during model inference.                                                                           |
+
+Supported models (see the [OpenLM Research OpenLLaMa GitHub repo](https://github.com/openlm-research/open_llama) for details):
+
+- `"openlm-research/open_llama_3b_350bt_preview"`
+- `"openlm-research/open_llama_3b_600bt_preview"`
+- `"openlm-research/open_llama_7b_400bt_preview"`
+- `"openlm-research/open_llama_7b_700bt_preview"`
+
+Note that Hugging Face will download this model the first time you use it - you can
+[define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
+by setting the environmental variable `HF_HOME`.
+
 ### Cache
 
 Interacting with LLMs, either through an external API or a local instance, is costly.
 Since developing an NLP pipeline generally means a lot of exploration and prototyping,
 `spacy-llm` implements a built-in cache to avoid reprocessing the same documents at each run.
 
 Example config block:
```

#### html2text {}

```diff
@@ -1,29 +1,12 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.2.1 Summary: Integrating LLMs
-into structured NLP pipelines Author: Explosion Author-email:
-contact@explosion.ai License: MIT Project-URL: Release notes, https://
-github.com/explosion/spacy-llm/releases Project-URL: Source, https://
-github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: minichain Provides-Extra: langchain
-Provides-Extra: transformers License-File: LICENSE [https://explosion.ai/
-assets/img/logo.svg] # spacy-llm: Integrating LLMs into structured NLP
-pipelines [![GitHub Workflow Status](https://img.shields.io/github/actions/
-workflow/status/explosion/spacy-llm/test.yml?branch=main)](https://github.com/
-explosion/spacy-llm/actions/workflows/test.yml) [![pypi Version](https://
-img.shields.io/pypi/v/spacy-llm.svg?style=flat-
+[https://explosion.ai/assets/img/logo.svg] # spacy-llm: Integrating LLMs into
+structured NLP pipelines [![GitHub Workflow Status](https://img.shields.io/
+github/actions/workflow/status/explosion/spacy-llm/test.yml?branch=main)]
+(https://github.com/explosion/spacy-llm/actions/workflows/test.yml) [![pypi
+Version](https://img.shields.io/pypi/v/spacy-llm.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy-llm/) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-
 000000.svg?style=flat-square)](https://github.com/ambv/black) This package
 integrates Large Language Models (LLMs) into [spaCy](https://spacy.io),
 featuring a modular system for **fast prototyping** and **prompting**, and
 turning unstructured responses into **robust outputs** for various NLP tasks,
 **no training data** required. - Serializable `llm` **component** to integrate
@@ -89,15 +72,15 @@
 Hugging Face To run this example, ensure that you have a GPU enabled, and
 `transformers`, `torch` and CUDA installed. For more background information,
 see the [DollyHF](#spacydollyhfv1) section. Create a config file `config.cfg`
 containing at least the following (or see the full example [here]
 (usage_examples/ner_dolly)): ```ini [nlp] lang = "en" pipeline = ["llm"]
 [components] [components.llm] factory = "llm" [components.llm.task] @llm_tasks
 = "spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"]
-[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" # For better
+[components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1" # For better
 performance, use databricks/dolly-v2-12b instead model = "databricks/dolly-v2-
 3b" ``` Now run: ```python from spacy_llm.util import assemble nlp = assemble
 ("config.cfg") doc = nlp("Jack and Jill rode up the hill in Les Deux Alpes")
 print([(ent.text, ent.label_) for ent in doc.ents]) ``` Note that Hugging Face
 will download the `"databricks/dolly-v2-3b"` model the first time you use it.
 You can [define the cached directory](https://huggingface.co/docs/
 huggingface_hub/main/en/guides/manage-cache) by setting the environmental
@@ -128,63 +111,100 @@
 my_other_config_val: float) -> "MyTask": labels_list = split_labels(labels)
 return MyTask(labels=labels_list, my_other_config_val=my_other_config_val)
 class MyTask: def __init__(self, labels: List[str], my_other_config_val:
 float): ... def generate_prompts(self, docs: Iterable[Doc]) -> Iterable[str]:
 ... def parse_responses( self, docs: Iterable[Doc], responses: Iterable[str] )
 -> Iterable[Doc]: ... ``` ```ini # config.cfg (excerpt) [components.llm.task]
 @llm_tasks = "my_namespace.MyTask.v1" labels = LABEL1,LABEL2,LABEL3
-my_other_config_val = 0.3 ``` ## ð API Each `llm` component is defined by
-two main settings: - A [**task**](#tasks), defining the prompt to send to the
-LLM as well as the functionality to parse the resulting response back into
-structured fields on spaCy's [Doc](https://spacy.io/api/doc) objects. - A
-[**backend**](#backends) defining the model to use and how to connect to it.
-Note that `spacy-llm` supports both access to external APIs (such as OpenAI) as
-well as access to self-hosted open-source LLMs (such as using Dolly through
-Hugging Face). Moreover, the component also implements [**caching**](#cache)
+my_other_config_val = 0.3 ``` ## Logging spacy-llm has a built-in logger that
+can log the prompt sent to the LLM as well as its raw response. This logger
+uses the debug level and by default has a `logging.NullHandler()` configured.
+In order to use this logger, you can setup a simple handler like this:
+```python import logging import spacy_llm spacy_llm.logger.addHandler
+(logging.StreamHandler()) spacy_llm.logger.setLevel(logging.DEBUG) ``` > NOTE:
+Any `logging` handler will work here so you probably want to use some sort of
+rotating `FileHandler` as the generated prompts can be quite long, especially
+for tasks with few-shot examples. Then when using the pipeline you'll be able
+to view the prompt and response. E.g. with the config and code from [Example 1]
+(##example-1-add-a-text-classifier-using-a-gpt-3-model-from-openai) above:
+```python from spacy_llm.util import assemble nlp = assemble("config.cfg") doc
+= nlp("You look gorgeous!") print(doc.cats) ``` You will see `logging` output
+similar to: ``` Generated prompt for doc: You look gorgeous! You are an expert
+Text Classification system. Your task is to accept Text as input and provide a
+category for the text based on the predefined labels. Classify the text below
+to any of the following labels: COMPLIMENT, INSULT The task is non-exclusive,
+so you can provide more than one label as long as they're comma-delimited. For
+example: Label1, Label2, Label3. Do not put any other text in your answer, only
+one or more of the provided labels with nothing before or after. If the text
+cannot be classified into any of the provided labels, answer `==NONE==`. Here
+is the text that needs classification Text: ''' You look gorgeous! ''' Backend
+response for doc: You look gorgeous! COMPLIMENT ``` `print(doc.cats)` to
+standard output should look like: ``` {'COMPLIMENT': 1.0, 'INSULT': 0.0} ``` ##
+ð API `spacy-llm` exposes a `llm` factory that accepts the following
+configuration options: | Argument | Type | Description | | --------- | --------
+----------------------------------- | -----------------------------------------
+------------------------------------------ | | `task` | `Optional[LLMTask]` |
+An LLMTask can generate prompts and parse LLM responses. See [docs](#tasks). |
+| `backend` | `Callable[[Iterable[Any]], Iterable[Any]]]` | Callable querying a
+specific LLM API. See [docs](#backends). | | `cache` | `Cache` | Cache to use
+for caching prompts and responses per doc (batch). See [docs](#cache). | |
+`save_io` | `bool` | Whether to save prompts/responses within `Doc.user_data
+["llm_io"]` | An `llm` component is defined by two main settings: - A
+[**task**](#tasks), defining the prompt to send to the LLM as well as the
+functionality to parse the resulting response back into structured fields on
+spaCy's [Doc](https://spacy.io/api/doc) objects. - A [**backend**](#backends)
+defining the model to use and how to connect to it. Note that `spacy-llm`
+supports both access to external APIs (such as OpenAI) as well as access to
+self-hosted open-source LLMs (such as using Dolly through Hugging Face).
+Moreover, `spacy-llm` exposes a customizable [**caching**](#cache)
 functionality to avoid running the same document through an LLM service (be it
-local or through a REST API) more than once. ### Tasks A _task_ defines an NLP
-problem or question, that will be sent to the LLM via a prompt. Further, the
-task defines how to parse the LLM's responses back into structured information.
-All tasks are registered in spaCy's `llm_tasks` registry. Practically speaking,
-a task should adhere to the `Protocol` `LLMTask` defined in [`ty.py`]
-(spacy_llm/ty.py). It needs to define a `generate_prompts` function and a
-`parse_responses` function. Moreover, the task may define an optional [`scorer`
-method](https://spacy.io/api/scorer#score). It should accept an iterable of
-`Example`s as input and return a score dictionary. If the `scorer` method is
-defined, `spacy-llm` will call it to evaluate the component. #### function
-`task.generate_prompts` Takes a collection of documents, and returns a
-collection of "prompts", which can be of type `Any`. Often, prompts are of type
-`str` - but this is not enforced to allow for maximum flexibility in the
-framework. | Argument | Type | Description | | ----------- | --------------- |
----------------------- | | `docs` | `Iterable[Doc]` | The input documents. | |
-**RETURNS** | `Iterable[Any]` | The generated prompts. | #### function
-`task.parse_responses` Takes a collection of LLM responses and the original
-documents, parses the responses into structured information, and sets the
-annotations on the documents. The `parse_responses` function is free to set the
-annotations in any way, including `Doc` fields like `ents`, `spans` or `cats`,
-or using custom defined fields. The `responses` are of type `Iterable[Any]`,
-though they will often be `str` objects. This depends on the return type of the
-[backend](#backends). | Argument | Type | Description | | ----------- | -------
--------- | ------------------------ | | `docs` | `Iterable[Doc]` | The input
-documents. | | `responses` | `Iterable[Any]` | The generated prompts. | |
-**RETURNS** | `Iterable[Doc]` | The annotated documents. | #### spacy.NER.v2
-The built-in NER task supports both zero-shot and few-shot prompting. This
-version also supports explicitly defining the provided labels with custom
-descriptions. ```ini [components.llm.task] @llm_tasks = "spacy.NER.v2" labels =
-["PERSON", "ORGANISATION", "LOCATION"] examples = null ``` | Argument | Type |
-Default | Description | | ------------------------- | -------------------------
--------------- | -------------------------------------------------------- | ---
+local or through a REST API) more than once. Finally, you can choose to save a
+stringified version of LLM prompts/responses within the `Doc.user_data
+["llm_io"]` attribute by setting `save_io` to `True`. `Doc.user_data["llm_io"]`
+is a dictionary containing one entry for every LLM component within the spaCy
+pipeline. Each entry is itself a dictionary, with two keys: `prompt` and
+`response`. ### Tasks A _task_ defines an NLP problem or question, that will be
+sent to the LLM via a prompt. Further, the task defines how to parse the LLM's
+responses back into structured information. All tasks are registered in spaCy's
+`llm_tasks` registry. Practically speaking, a task should adhere to the
+`Protocol` `LLMTask` defined in [`ty.py`](spacy_llm/ty.py). It needs to define
+a `generate_prompts` function and a `parse_responses` function. Moreover, the
+task may define an optional [`scorer` method](https://spacy.io/api/
+scorer#score). It should accept an iterable of `Example`s as input and return a
+score dictionary. If the `scorer` method is defined, `spacy-llm` will call it
+to evaluate the component. #### function `task.generate_prompts` Takes a
+collection of documents, and returns a collection of "prompts", which can be of
+type `Any`. Often, prompts are of type `str` - but this is not enforced to
+allow for maximum flexibility in the framework. | Argument | Type | Description
+| | ----------- | --------------- | ---------------------- | | `docs` |
+`Iterable[Doc]` | The input documents. | | **RETURNS** | `Iterable[Any]` | The
+generated prompts. | #### function `task.parse_responses` Takes a collection of
+LLM responses and the original documents, parses the responses into structured
+information, and sets the annotations on the documents. The `parse_responses`
+function is free to set the annotations in any way, including `Doc` fields like
+`ents`, `spans` or `cats`, or using custom defined fields. The `responses` are
+of type `Iterable[Any]`, though they will often be `str` objects. This depends
+on the return type of the [backend](#backends). | Argument | Type | Description
+| | ----------- | --------------- | ------------------------ | | `docs` |
+`Iterable[Doc]` | The input documents. | | `responses` | `Iterable[Any]` | The
+generated prompts. | | **RETURNS** | `Iterable[Doc]` | The annotated documents.
+| #### spacy.NER.v2 The built-in NER task supports both zero-shot and few-shot
+prompting. This version also supports explicitly defining the provided labels
+with custom descriptions. ```ini [components.llm.task] @llm_tasks =
+"spacy.NER.v2" labels = ["PERSON", "ORGANISATION", "LOCATION"] examples = null
+``` | Argument | Type | Default | Description | | ------------------------- | -
+-------------------------------------- | --------------------------------------
+------------------ | ----------------------------------------------------------
 -------------------------------------------------------------------------------
-------------------------------------------------------------------- | |
-`labels` | `Union[List[str], str]` | | List of labels or str of comma-separated
-list of labels. | | `template` | `str` | [ner.v2.jinja](./spacy_llm/tasks/
-templates/ner.v2.jinja) | Custom prompt template to send to LLM backend.
-Default templates for each task are located in the `spacy_llm/tasks/templates`
-directory. | | `label_definitions` | `Optional[Dict[str, str]]` | `None` |
-Optional dict mapping a label to a description of that label. These
+------------ | | `labels` | `Union[List[str], str]` | | List of labels or str
+of comma-separated list of labels. | | `template` | `str` | [ner.v2.jinja](./
+spacy_llm/tasks/templates/ner.v2.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `label_definitions` | `Optional[Dict[str, str]]` |
+`None` | Optional dict mapping a label to a description of that label. These
 descriptions are added to the prompt to help instruct the LLM on what to
 extract. | | `examples` | `Optional[Callable[[], Iterable[Any]]]` | `None` |
 Optional function that generates examples for few-shot learning. | |
 `normalizer` | `Optional[Callable[[str], str]]` | `None` | Function that
 normalizes the labels as returned by the LLM. If `None`, defaults to
 `spacy.LowercaseNormalizer.v1`. | | `alignment_mode` | `str` | `"contract"` |
 Alignment mode in case the LLM returns entities that do not align with token
@@ -401,147 +421,226 @@
 "end_char": 7, "label": "PERSON"}, {"start_char": 26, "end_char": 39, "label":
 "LOC"}], "relations": [{"dep": 0, "dest": 1, "relation": "Visits"}]} ``` Note:
 the REL task relies on pre-extracted entities to make its prediction. Hence,
 you'll need to add a component that populates `doc.ents` with recognized spans
 to your spaCy pipeline and put it _before_ the REL component. ```ini
 [components.llm.task] @llm_tasks = "spacy.REL.v1" labels = ["LivesIn",
 "Visits"] [components.llm.task.examples] @misc = "spacy.FewShotReader.v1" path
-= "rel_examples.jsonl" ``` #### spacy.NoOp.v1 This task is only useful for
-testing - it tells the LLM to do nothing, and does not set any fields on the
-`docs`. ```ini [components.llm.task] @llm_tasks = "spacy.NoOp.v1" ``` ###
-Backends A _backend_ defines which LLM model to query, and how to query it. It
-can be a simple function taking a collection of prompts (consistent with the
-output type of `task.generate_prompts()`) and returning a collection of
-responses (consistent with the expected input of `parse_responses`). Generally
-speaking, it's a function of type `Callable[[Iterable[Any]], Iterable[Any]]`,
-but specific implementations can have other signatures, like `Callable[
-[Iterable[str]], Iterable[str]]`. All built-in backends are registered in
-`llm_backends`. If no backend is specified, the repo currently connects to the
-[`OpenAI` API](#openai) by default, using the built-in REST protocol, and
-accesses the `"gpt-3.5-turbo"` model. > :question: _Why are there backends for
-third-party libraries in addition to a native REST backend and which should > I
-choose?_ > > Third-party libraries like `langchain` or `minichain` focus on
-prompt management, integration of many different LLM > APIs, and other related
-features such as conversational memory or agents. `spacy-llm` on the other hand
-emphasizes > features we consider useful in the context of NLP pipelines
-utilizing LLMs to process documents (mostly) independent > from each other. It
-makes sense that the feature set of such third-party libraries and `spacy-llm`
-is not identical - > and users might want to take advantage of features not
-available in `spacy-llm`. > > The advantage of offering our own REST backend is
-that we can ensure a larger degree of stability of robustness, as > we can
-guarantee backwards-compatibility and more smoothly integrated error handling.
-> > Ultimately we recommend trying to implement your use case using the REST
-backend first (which is configured as the > default backend). If however there
-are features or APIs not covered by `spacy-llm`, it's trivial to switch to the
-> backend of a third-party library - and easy to customize the prompting
-mechanism, if so required. #### OpenAI When the backend uses OpenAI, you have
-to get an API key from openai.com, and ensure that the keys are set as
-environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
-OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
-`requests` and a simple retry mechanism to access an API. ```ini
-[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
-= {"model": "gpt-3.5-turbo", "temperature": 0.3} ``` | Argument | Type |
-Default | Description | | ----------- | ---------------- | ------- | ----------
+= "rel_examples.jsonl" ``` #### spacy.Lemma.v1 The `Lemma.v1` task lemmatizes
+the provided text and updates the `lemma_` attribute in the doc's tokens
+accordingly. ```ini [components.llm.task] @llm_tasks = "spacy.Lemma.v1"
+examples = null ``` | Argument | Type | Default | Description | | -------------
+------------ | --------------------------------------- |-----------------------
+------------------------------------| -----------------------------------------
 -------------------------------------------------------------------------------
---------------------------- | | `api` | `str` | | The name of a supported API.
-In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
-| Further configuration passed on to the backend. | | `strict` | `bool` |
-`True` | If `True`, raises an error if the LLM API returns a malformed
-response. Otherwise, return the error responses as is. | | `max_tries` | `int`
-| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
-Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
-following settings can be defined in the `config` dictionary: - `model`: one of
-the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
-`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
-babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
-`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
-For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
-completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
-srush/MiniChain) for the API retrieval part, make sure you have installed it
-first: ```shell python -m pip install "minichain>=0.3,<0.4" # Or install with
-spacy-llm directly python -m pip install "spacy-llm[minichain]" ``` Note that
-MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
-blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
-api = "OpenAI" [components.llm.backend.query] @llm_queries =
-"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
---- | -------------------------------------------------------------------------
--------- | ------- | ----------------------------------------------------------
-------------------------- | | `api` | `str` | | The name of an API supported by
-MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
-configuration passed on to the backend. | | `query` | `Optional[Callable[
-["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
-Function that executes the prompts. If `None`, defaults to
-`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
-executes the prompts by running `model(text).run()` for each given textual
-prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
-hwchase17/langchain) for the API retrieval part, make sure you have installed
-it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" # Or install
-with spacy-llm directly python -m pip install "spacy-llm[langchain]" ``` Note
-that LangChain currently only supports Python 3.9 and beyond. Example config
-block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
-= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
-{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
-- | ---------------------------------------------------------------------------
---- | ------- | ---------------------------------------------------------------
---------------------- | | `api` | `str` | | The name of an API supported by
-LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
-configuration passed on to the backend. | | `query` | `Optional[Callable[
-["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
-that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
-The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
-`model(text)` for each given textual prompt. #### spacy.DollyHF.v1 To use this
+----------------------------- | | `template` | `str` | [lemma.jinja](./
+spacy_llm/tasks/templates/lemma.jinja) | Custom prompt template to send to LLM
+backend. Default templates for each task are located in the `spacy_llm/tasks/
+templates` directory. | | `examples` | `Optional[Callable[[], Iterable[Any]]]`
+| `None` | Optional function that generates examples for few-shot learning. |
+`Lemma.v1` prompts the LLM to lemmatize the passed text and return the
+lemmatized version as a list of tokens and their corresponding lemma. E. g. the
+text `I'm buying ice cream for my friends` should invoke the response ``` I: I
+'m: be buying: buy ice: ice cream: cream for: for my: my friends: friend .: .
+``` If for any given text/doc instance the number of lemmas returned by the LLM
+doesn't match the number of tokens recognized by spaCy, no lemmas are stored in
+the corresponding doc's tokens. Otherwise the tokens `.lemma_` property is
+updated with the lemma suggested by the LLM. To perform few-shot learning, you
+can write down a few examples in a separate file, and provide these to be
+injected into the prompt to the LLM. The default reader
+`spacy.FewShotReader.v1` supports `.yml`, `.yaml`, `.json` and `.jsonl`.
+```yaml - text: I'm buying ice cream. lemmas: - "I": "I" - "'m": "be" -
+"buying": "buy" - "ice": "ice" - "cream": "cream" - ".": "." - text: I've
+watered the plants. lemmas: - "I": "I" - "'ve": "have" - "watered": "water" -
+"the": "the" - "plants": "plant" - ".": "." ``` ```ini [components.llm.task]
+@llm_tasks = "spacy.Lemma.v1" [components.llm.task.examples] @misc =
+"spacy.FewShotReader.v1" path = "lemma_examples.yml" ``` #### spacy.NoOp.v1
+This task is only useful for testing - it tells the LLM to do nothing, and does
+not set any fields on the `docs`. ```ini [components.llm.task] @llm_tasks =
+"spacy.NoOp.v1" ``` ### Backends A _backend_ defines which LLM model to query,
+and how to query it. It can be a simple function taking a collection of prompts
+(consistent with the output type of `task.generate_prompts()`) and returning a
+collection of responses (consistent with the expected input of
+`parse_responses`). Generally speaking, it's a function of type `Callable[
+[Iterable[Any]], Iterable[Any]]`, but specific implementations can have other
+signatures, like `Callable[[Iterable[str]], Iterable[str]]`. All built-in
+backends are registered in `llm_backends`. If no backend is specified, the repo
+currently connects to the [`OpenAI` API](#openai) by default, using the built-
+in REST protocol, and accesses the `"gpt-3.5-turbo"` model. > :question: _Why
+are there backends for third-party libraries in addition to a native REST
+backend and which should > I choose?_ > > Third-party libraries like
+`langchain` or `minichain` focus on prompt management, integration of many
+different LLM > APIs, and other related features such as conversational memory
+or agents. `spacy-llm` on the other hand emphasizes > features we consider
+useful in the context of NLP pipelines utilizing LLMs to process documents
+(mostly) independent > from each other. It makes sense that the feature set of
+such third-party libraries and `spacy-llm` is not identical - > and users might
+want to take advantage of features not available in `spacy-llm`. > > The
+advantage of offering our own REST backend is that we can ensure a larger
+degree of stability of robustness, as > we can guarantee backwards-
+compatibility and more smoothly integrated error handling. > > Ultimately we
+recommend trying to implement your use case using the REST backend first (which
+is configured as the > default backend). If however there are features or APIs
+not covered by `spacy-llm`, it's trivial to switch to the > backend of a third-
+party library - and easy to customize the prompting mechanism, if so required.
+#### OpenAI When the backend uses OpenAI, you have to get an API key from
+openai.com, and ensure that the keys are set as environmental variables:
+```shell export OPENAI_API_KEY="sk-..." export OPENAI_API_ORG="org-..." ```
+#### spacy.REST.v1 This default backend uses `requests` and a simple retry
+mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
+"spacy.REST.v1" api = "OpenAI" config = {"model": "gpt-3.5-turbo",
+"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
+-- | ---------------- | ------- | ---------------------------------------------
+----------------------------------------------------------------------- | |
+`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
+supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
+passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
+error if the LLM API returns a malformed response. Otherwise, return the error
+responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
+request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
+When `api` is set to `OpenAI`, the following settings can be defined in the
+`config` dictionary: - `model`: one of the following list of supported models:
+- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
+turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
+- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
+`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
+api.openai.com/v1/completions`. For models requiring the chat endpoint, use
+`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
+[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
+make sure you have installed it first: ```shell python -m pip install
+"minichain>=0.3,<0.4" # Or install with spacy-llm directly python -m pip
+install "spacy-llm[minichain]" ``` Note that MiniChain currently only supports
+Python 3.8, 3.9 and 3.10. Example config blocks: ```ini
+[components.llm.backend] @llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
+[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
+Argument | Type | Default | Description | | -------- | ------------------------
+--------------------------------------------------------- | ------- | ---------
+-------------------------------------------------------------------------- | |
+`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
+`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
+backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
+Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
+If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
+(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
+for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
+(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
+you have installed it first: ```shell python -m pip install
+"langchain>=0.0.144,<0.1" # Or install with spacy-llm directly python -m pip
+install "spacy-llm[langchain]" ``` Note that LangChain currently only supports
+Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
+@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
+"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
+Default | Description | | -------- | ------------------------------------------
+------------------------------------ | ------- | ------------------------------
+------------------------------------------------------ | | `api` | `str` | |
+The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
+[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
+`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
+Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
+defaults to `spacy.CallLangChain.v1`. | The default `query`
+(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
+each given textual prompt. #### spacy.Dolly_HF.v1 To use this backend, ideally
+you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
+your virtual environment. This allows you to have the setting `device=cuda:0`
+in your config, which ensures that the model is loaded entirely on the GPU (and
+fails otherwise). You can do so with ```shell python -m pip install "spacy-llm
+[transformers]" "transformers[sentencepiece]" ``` If you don't have access to a
+GPU, you can install `accelerate` and set`device_map=auto` instead, but be
+aware that this may result in some layers getting distributed to the CPU or
+even the hard drive, which may ultimately result in extremely slow queries.
+```shell python -m pip install "accelerate>=0.16.0,<1.0" ``` Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.Dolly_HF.v1"
+model = "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description
+| | ------------- | ---------------- | ------- | ------------------------------
+------------------------------------------------------------------ | | `model`
+| `str` | | The name of a Dolly model that is supported. | | `config_init` |
+`Dict[str, Any]` | `{}` | Further configuration passed on to the construction
+of the model with `transformers.pipeline()`. | | `config_run` | `Dict[str,
+Any]` | `{}` | Further configuration used during model inference. | Supported
+models (see the [Databricks models page](https://huggingface.co/databricks) on
+Hugging Face for details): - `"databricks/dolly-v2-3b"` - `"databricks/dolly-
+v2-7b"` - `"databricks/dolly-v2-12b"` Note that Hugging Face will download this
+model the first time you use it - you can [define the cached directory](https:/
+/huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting
+the environmental variable `HF_HOME`. #### spacy.StableLM_HF.v1 To use this
 backend, ideally you have a GPU enabled and have installed `transformers`,
-`torch` and CUDA in your virtual environment. This allows you to have the
-setting `device=cuda:0` in your config, which ensures that the model is loaded
-entirely on the GPU (and fails otherwise). ```shell python -m pip install
-"torch>=1.13.1,<2.0" python -m pip install "transformers>=4.28.1,<5.0" # Or
-install with spacy-llm directly python -m pip install "spacy-llm[transformers]"
+`torch` and CUDA in your virtual environment. You can do so with ```shell
+python -m pip install "spacy-llm[transformers]" "transformers[sentencepiece]"
 ``` If you don't have access to a GPU, you can install `accelerate` and
 set`device_map=auto` instead, but be aware that this may result in some layers
 getting distributed to the CPU or even the hard drive, which may ultimately
 result in extremely slow queries. ```shell python -m pip install
 "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
-[components.llm.backend] @llm_backends = "spacy.DollyHF.v1" model =
-"databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
----- | ---------------- | ------- | -------------------------------------------
------------------------------------------------------ | | `model` | `str` | |
-The name of a Dolly model that is supported. | | `config` | `Dict[Any, Any]` |
-`{}` | Further configuration passed on to the construction of the model with
-`transformers.pipeline()`. | Supported models (see the [Databricks models page]
-(https://huggingface.co/databricks) on Hugging Face for details): -
-`"databricks/dolly-v2-3b"` - `"databricks/dolly-v2-7b"` - `"databricks/dolly-
-v2-12b"` Note that Hugging Face will download this model the first time you use
-it - you can [define the cached directory](https://huggingface.co/docs/
+[components.llm.backend] @llm_backends = "spacy.StableLM_HF.v1" model =
+"stabilityai/stablelm-tuned-alpha-7b" ``` | Argument | Type | Default |
+Description | | ------------- | ---------------- | ------- | ------------------
+-------------------------------------------------------------------------------
+--------------------------- | | `model` | `str` | | The name of a StableLM
+model that is supported. | | `config_init` | `Dict[str, Any]` | `{}` | Further
+configuration passed on to the construction of the model with
+`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
+[str, Any]` | `{}` | Further configuration used during model inference. |
+Supported models (see the [Stability AI StableLM GitHub repo](https://
+github.com/Stability-AI/StableLM/#stablelm-alpha) for details): -
+`"stabilityai/stablelm-base-alpha-3b"` - `"stabilityai/stablelm-base-alpha-7b"`
+- `"stabilityai/stablelm-tuned-alpha-3b"` - `"stabilityai/stablelm-tuned-alpha-
+7b"` Note that Hugging Face will download this model the first time you use it
+- you can [define the cached directory](https://huggingface.co/docs/
 huggingface_hub/main/en/guides/manage-cache) by setting the environmental
-variable `HF_HOME`. ### Cache Interacting with LLMs, either through an external
-API or a local instance, is costly. Since developing an NLP pipeline generally
-means a lot of exploration and prototyping, `spacy-llm` implements a built-in
-cache to avoid reprocessing the same documents at each run. Example config
-block: ```ini [components.llm.cache] @llm_misc = "spacy.BatchCache.v1", path =
-"path/to/cache" batch_size = 64 max_batches_in_mem = 4 ``` | Argument | Type |
-Default | Description | | -------------------- | ---------------------------- |
-------- | ---------------------------------------------------- | | `path` |
-`Optional[Union[str, Path]]` | `None` | Cache directory. If `None`, no caching
-is performed. | | `batch_size` | `int` | 64 | Number of docs in one batch
-(file). | | `max_batches_in_mem` | `int` | 4 | Max. number of batches to hold
-in memory. | Note that since the cache is generated by a registered function,
-you can also provide your own registered function returning your own cache
-implementation. If you wish to do so, ensure that your cache object adheres to
-the `Protocol` defined in `spacy_llm.ty.Cache`. ### Various functions ####
-spacy.FewShotReader.v1 This function is registered in spaCy's `misc` registry,
-and reads in examples from a `.yml`, `.yaml`, `.json` or `.jsonl` file. It uses
-[`srsly`](https://github.com/explosion/srsly) to read in these files and parses
-them depending on the file extension. ```ini [components.llm.task.examples]
-@misc = "spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument |
-Type | Description | | -------- | ------------------ | ------------------------
--------------------------------------------------- | | `path` | `Union[str,
-Path]` | Path to an examples file with suffix `.yml`, `.yaml`, `.json` or
-`.jsonl`. | #### spacy.FileReader.v1 This function is registered in spaCy's
-`misc` registry, and reads a file provided to the `path` to return a `str`
+variable `HF_HOME`. #### spacy.OpenLLaMaHF.v1 To use this backend, ideally you
+have a GPU enabled and have installed - `transformers[sentencepiece]` - `torch`
+- CUDA in your virtual environment. You can do so with ```shell python -m pip
+install "spacy-llm[transformers]" "transformers[sentencepiece]" ``` If you
+don't have access to a GPU, you can install `accelerate` and
+set`device_map=auto` instead, but be aware that this may result in some layers
+getting distributed to the CPU or even the hard drive, which may ultimately
+result in extremely slow queries. ```shell python -m pip install
+"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+[components.llm.backend] @llm_backends = "spacy.OpenLLaMaHF.v1" model =
+"openlm-research/open_llama_3b_350bt_preview" ``` | Argument | Type | Default |
+Description | | ------------- | ---------------- | ------- | ------------------
+-------------------------------------------------------------------------------
+--------------------------- | | `model` | `str` | | The name of a OpenLLaMa
+model that is supported. | | `config_init` | `Dict[str, Any]` | `{}` | Further
+configuration passed on to the construction of the model with
+`transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
+[str, Any]` | `{}` | Further configuration used during model inference. |
+Supported models (see the [OpenLM Research OpenLLaMa GitHub repo](https://
+github.com/openlm-research/open_llama) for details): - `"openlm-research/
+open_llama_3b_350bt_preview"` - `"openlm-research/open_llama_3b_600bt_preview"`
+- `"openlm-research/open_llama_7b_400bt_preview"` - `"openlm-research/
+open_llama_7b_700bt_preview"` Note that Hugging Face will download this model
+the first time you use it - you can [define the cached directory](https://
+huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache) by setting the
+environmental variable `HF_HOME`. ### Cache Interacting with LLMs, either
+through an external API or a local instance, is costly. Since developing an NLP
+pipeline generally means a lot of exploration and prototyping, `spacy-llm`
+implements a built-in cache to avoid reprocessing the same documents at each
+run. Example config block: ```ini [components.llm.cache] @llm_misc =
+"spacy.BatchCache.v1", path = "path/to/cache" batch_size = 64
+max_batches_in_mem = 4 ``` | Argument | Type | Default | Description | | ------
+-------------- | ---------------------------- | ------- | ---------------------
+------------------------------- | | `path` | `Optional[Union[str, Path]]` |
+`None` | Cache directory. If `None`, no caching is performed. | | `batch_size`
+| `int` | 64 | Number of docs in one batch (file). | | `max_batches_in_mem` |
+`int` | 4 | Max. number of batches to hold in memory. | Note that since the
+cache is generated by a registered function, you can also provide your own
+registered function returning your own cache implementation. If you wish to do
+so, ensure that your cache object adheres to the `Protocol` defined in
+`spacy_llm.ty.Cache`. ### Various functions #### spacy.FewShotReader.v1 This
+function is registered in spaCy's `misc` registry, and reads in examples from a
+`.yml`, `.yaml`, `.json` or `.jsonl` file. It uses [`srsly`](https://
+github.com/explosion/srsly) to read in these files and parses them depending on
+the file extension. ```ini [components.llm.task.examples] @misc =
+"spacy.FewShotReader.v1" path = "ner_examples.yml" ``` | Argument | Type |
+Description | | -------- | ------------------ | -------------------------------
+------------------------------------------- | | `path` | `Union[str, Path]` |
+Path to an examples file with suffix `.yml`, `.yaml`, `.json` or `.jsonl`. |
+#### spacy.FileReader.v1 This function is registered in spaCy's `misc`
+registry, and reads a file provided to the `path` to return a `str`
 representation of its contents. This function is typically used to read [Jinja]
 (https://jinja.palletsprojects.com/en/3.1.x/) files containing the prompt
 template. ```ini [components.llm.task.template] @misc = "spacy.FileReader.v1"
 path = "ner_template.jinja2" ``` | Argument | Type | Description | | -------- |
 ------------------ | ---------------------------- | | `path` | `Union[str,
 Path]` | Path to the file to be read. | #### Normalizer functions These
 functions provide simple normalizations for string comparisons, e.g. between a
```

### Comparing `spacy-llm-0.2.1/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.3.0/spacy_llm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,80 +14,98 @@
 spacy_llm.egg-info/dependency_links.txt
 spacy_llm.egg-info/entry_points.txt
 spacy_llm.egg-info/not-zip-safe
 spacy_llm.egg-info/requires.txt
 spacy_llm.egg-info/top_level.txt
 spacy_llm/backends/__init__.py
 spacy_llm/backends/integration/__init__.py
-spacy_llm/backends/integration/base.py
-spacy_llm/backends/integration/dolly.py
-spacy_llm/backends/integration/langchain.py
-spacy_llm/backends/integration/minichain.py
+spacy_llm/backends/integration/hf/__init__.py
+spacy_llm/backends/integration/hf/base.py
+spacy_llm/backends/integration/hf/dolly.py
+spacy_llm/backends/integration/hf/openllama.py
+spacy_llm/backends/integration/hf/stablelm.py
+spacy_llm/backends/integration/remote/__init__.py
+spacy_llm/backends/integration/remote/base.py
+spacy_llm/backends/integration/remote/langchain.py
+spacy_llm/backends/integration/remote/minichain.py
 spacy_llm/backends/rest/__init__.py
+spacy_llm/backends/rest/anthropic.py
+spacy_llm/backends/rest/base.py
+spacy_llm/backends/rest/cohere.py
+spacy_llm/backends/rest/noop.py
+spacy_llm/backends/rest/openai.py
 spacy_llm/backends/rest/registry.py
-spacy_llm/backends/rest/backend/__init__.py
-spacy_llm/backends/rest/backend/base.py
-spacy_llm/backends/rest/backend/noop.py
-spacy_llm/backends/rest/backend/openai.py
 spacy_llm/pipeline/__init__.py
 spacy_llm/pipeline/llm.py
 spacy_llm/registry/__init__.py
 spacy_llm/registry/normalizer.py
 spacy_llm/registry/reader.py
 spacy_llm/registry/util.py
 spacy_llm/tasks/__init__.py
+spacy_llm/tasks/lemma.py
 spacy_llm/tasks/ner.py
 spacy_llm/tasks/noop.py
 spacy_llm/tasks/rel.py
 spacy_llm/tasks/spancat.py
 spacy_llm/tasks/textcat.py
 spacy_llm/tasks/templates/__init__.py
+spacy_llm/tasks/templates/lemma.jinja
 spacy_llm/tasks/templates/ner.jinja
 spacy_llm/tasks/templates/ner.v2.jinja
 spacy_llm/tasks/templates/rel.jinja
 spacy_llm/tasks/templates/spancat.jinja
 spacy_llm/tasks/templates/spancat.v2.jinja
 spacy_llm/tasks/templates/textcat.jinja
 spacy_llm/tasks/templates/textcat.v2.jinja
 spacy_llm/tasks/templates/textcat.v3.jinja
 spacy_llm/tasks/util/__init__.py
 spacy_llm/tasks/util/examples.py
 spacy_llm/tasks/util/parsing.py
+spacy_llm/tasks/util/serialization.py
 spacy_llm/tasks/util/span.py
 spacy_llm/tests/__init__.py
 spacy_llm/tests/compat.py
 spacy_llm/tests/conftest.py
 spacy_llm/tests/test_cache.py
 spacy_llm/tests/test_combinations.py
 spacy_llm/tests/test_registry.py
 spacy_llm/tests/backends/__init__.py
+spacy_llm/tests/backends/test_anthropic.py
+spacy_llm/tests/backends/test_cohere.py
 spacy_llm/tests/backends/test_dolly.py
 spacy_llm/tests/backends/test_langchain.py
 spacy_llm/tests/backends/test_minichain.py
+spacy_llm/tests/backends/test_openllama.py
 spacy_llm/tests/backends/test_rest.py
+spacy_llm/tests/backends/test_stablelm.py
 spacy_llm/tests/pipeline/__init__.py
 spacy_llm/tests/pipeline/test_llm.py
 spacy_llm/tests/tasks/__init__.py
+spacy_llm/tests/tasks/test_lemma.py
 spacy_llm/tests/tasks/test_ner.py
 spacy_llm/tests/tasks/test_rel.py
 spacy_llm/tests/tasks/test_spancat.py
 spacy_llm/tests/tasks/test_textcat.py
+spacy_llm/tests/tasks/examples/lemma_examples.json
+spacy_llm/tests/tasks/examples/lemma_examples.jsonl
+spacy_llm/tests/tasks/examples/lemma_examples.yml
 spacy_llm/tests/tasks/examples/ner_examples.json
 spacy_llm/tests/tasks/examples/ner_examples.jsonl
 spacy_llm/tests/tasks/examples/ner_examples.yml
 spacy_llm/tests/tasks/examples/rel_examples.jsonl
 spacy_llm/tests/tasks/examples/textcat_binary_examples.json
 spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
 spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
 spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
 spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
 spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
 spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
 spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
 spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+spacy_llm/tests/tasks/templates/lemma_template.jinja2
 spacy_llm/tests/tasks/templates/ner_template.jinja2
 spacy_llm/tests/tasks/templates/textcat_template.jinja2
 usage_examples/__init__.py
 usage_examples/multitask_openai/__init__.py
 usage_examples/multitask_openai/run_pipeline.py
 usage_examples/ner_dolly/__init__.py
 usage_examples/ner_dolly/run_pipeline.py
```

### Comparing `spacy-llm-0.2.1/usage_examples/multitask_openai/run_pipeline.py` & `spacy-llm-0.3.0/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/usage_examples/ner_dolly/run_pipeline.py` & `spacy-llm-0.3.0/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy-llm-0.3.0/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/usage_examples/ner_minichain_openai/run_pipeline.py` & `spacy-llm-0.3.0/usage_examples/ner_minichain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/usage_examples/rel_openai/run_pipeline.py` & `spacy-llm-0.3.0/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/usage_examples/tests/test_readme_examples.py` & `spacy-llm-0.3.0/usage_examples/tests/test_readme_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         factory = "llm"
 
         [components.llm.task]
         @llm_tasks = "spacy.NER.v2"
         labels = ["PERSON", "ORGANISATION", "LOCATION"]
 
         [components.llm.backend]
-        @llm_backends = "spacy.DollyHF.v1"
+        @llm_backends = "spacy.Dolly_HF.v1"
         # For better performance, use databricks/dolly-v2-12b instead
         model = "databricks/dolly-v2-3b"
         """
 
         with open(tmpdir / "cfg", "w") as text_file:
             text_file.write(cfg_str)
```

### Comparing `spacy-llm-0.2.1/usage_examples/tests/test_usage_examples.py` & `spacy-llm-0.3.0/usage_examples/tests/test_usage_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.2.1/usage_examples/textcat_openai/run_pipeline.py` & `spacy-llm-0.3.0/usage_examples/textcat_openai/run_pipeline.py`

 * *Files identical despite different names*

