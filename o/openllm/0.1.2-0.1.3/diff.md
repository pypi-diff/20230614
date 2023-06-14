# Comparing `tmp/openllm-0.1.2.tar.gz` & `tmp/openllm-0.1.3.tar.gz`

## Comparing `openllm-0.1.2.tar` & `openllm-0.1.3.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 openllm-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.2/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 openllm-0.1.2/DEVELOPMENT.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.2/package.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.2/taplo.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/ISSUE_TEMPLATE/feature_request.yml
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/actions/create_release_and_archive.sh
--rwxr-xr-x   0        0        0     1764 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/actions/release.sh
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/actions/setup-repo/action.yml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/workflows/create-releases.yml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.2/.github/workflows/release-notes.yml
--rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.2/assets/output.gif
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 openllm-0.1.2/examples/play.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/__about__.py
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/__main__.py
--rw-r--r--   0        0        0    52649 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_configuration.py
--rw-r--r--   0        0        0    38314 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_llm.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_package.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_prompt.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_schema.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_service.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/_types.py
--rw-r--r--   0        0        0    40716 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/cli.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/client.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/py.typed
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0     9780 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/gptj/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/roberta/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/cache/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/cache/inmemory.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.2/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/test_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.2/tests/models/flan_t5/test_modeling_flan_t5.py
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/add-license-headers
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/assert-license-headers
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/assert-model-table-latest
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/run-release-action
--rwxr-xr-x   0        0        0     1844 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/update-optional-dependencies.py
--rwxr-xr-x   0        0        0     3389 2020-02-02 00:00:00.000000 openllm-0.1.2/tools/update-readme.py
--rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/__init__.pyi
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/_cmp.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/_compat.pyi
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/_typing_compat.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/_version_info.pyi
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/converters.pyi
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/exceptions.pyi
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/filters.pyi
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/setters.pyi
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/attr/validators.pyi
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/__init__.pyi
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/_core.pyi
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/_decorators.pyi
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/_helpers.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/click_option_group/_version.pyi
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/__init__.pyi
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/merger.pyi
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/strategy/core.pyi
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/strategy/dict.pyi
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/strategy/list.pyi
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.2/typings/deepmerge/strategy/set.pyi
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.1.2/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.2/LICENSE.md
--rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 openllm-0.1.2/README.md
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 openllm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    14717 2020-02-02 00:00:00.000000 openllm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 openllm-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.3/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 openllm-0.1.3/DEVELOPMENT.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.3/package.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.3/taplo.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/ISSUE_TEMPLATE/feature_request.yml
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/actions/create_release_and_archive.sh
+-rwxr-xr-x   0        0        0     1764 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/actions/release.sh
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/actions/setup-repo/action.yml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/workflows/create-releases.yml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.3/.github/workflows/release-notes.yml
+-rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.3/assets/output.gif
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 openllm-0.1.3/examples/play.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/__about__.py
+-rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/__main__.py
+-rw-r--r--   0        0        0    50213 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/_configuration.py
+-rw-r--r--   0        0        0    34895 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/_llm.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/_package.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/_schema.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/_service.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/_types.py
+-rw-r--r--   0        0        0    40654 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/cli.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/client.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/py.typed
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/gptj/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/roberta/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0    10442 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_client/cache/__init__.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_client/cache/inmemory.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.3/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 openllm-0.1.3/tests/test_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.3/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 openllm-0.1.3/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.3/tests/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.3/tests/models/flan_t5/test_modeling_flan_t5.py
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.3/tools/add-license-headers
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.3/tools/assert-license-headers
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 openllm-0.1.3/tools/assert-model-table-latest
+-rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.3/tools/run-release-action
+-rwxr-xr-x   0        0        0     1844 2020-02-02 00:00:00.000000 openllm-0.1.3/tools/update-optional-dependencies.py
+-rwxr-xr-x   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.3/tools/update-readme.py
+-rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/__init__.pyi
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/_cmp.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/_compat.pyi
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/_typing_compat.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/_version_info.pyi
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/converters.pyi
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/exceptions.pyi
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/filters.pyi
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/setters.pyi
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/attr/validators.pyi
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/click_option_group/__init__.pyi
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/click_option_group/_core.pyi
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/click_option_group/_decorators.pyi
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/click_option_group/_helpers.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/click_option_group/_version.pyi
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/deepmerge/__init__.pyi
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/deepmerge/merger.pyi
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/deepmerge/strategy/core.pyi
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/deepmerge/strategy/dict.pyi
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/deepmerge/strategy/list.pyi
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.3/typings/deepmerge/strategy/set.pyi
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 openllm-0.1.3/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 openllm-0.1.3/README.md
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 openllm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    16006 2020-02-02 00:00:00.000000 openllm-0.1.3/PKG-INFO
```

### Comparing `openllm-0.1.2/.pre-commit-config.yaml` & `openllm-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/ADDING_NEW_MODEL.md` & `openllm-0.1.3/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/DEVELOPMENT.md` & `openllm-0.1.3/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/package.json` & `openllm-0.1.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.1.2",
+    "version": "0.1.3",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.1.2/.github/dependabot.yml` & `openllm-0.1.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `openllm-0.1.3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/ISSUE_TEMPLATE/config.yml` & `openllm-0.1.3/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/ISSUE_TEMPLATE/feature_request.yml` & `openllm-0.1.3/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/actions/create_release_and_archive.sh` & `openllm-0.1.3/.github/actions/create_release_and_archive.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/actions/release.sh` & `openllm-0.1.3/.github/actions/release.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/actions/setup-repo/action.yml` & `openllm-0.1.3/.github/actions/setup-repo/action.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/workflows/ci.yml` & `openllm-0.1.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/workflows/create-releases.yml` & `openllm-0.1.3/.github/workflows/create-releases.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.github/workflows/release-notes.yml` & `openllm-0.1.3/.github/workflows/release-notes.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/assets/output.gif` & `openllm-0.1.3/assets/output.gif`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/examples/play.py` & `openllm-0.1.3/examples/play.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/__about__.py` & `openllm-0.1.3/src/openllm/models/gpt_neox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.2"
+
+raise NotImplementedError("This module is not implemented yet.")
```

### Comparing `openllm-0.1.2/src/openllm/__init__.py` & `openllm-0.1.3/src/openllm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     from bentoml._internal.log import configure_logging
 
     configure_logging()
     _.basicConfig(level=_.NOTSET)
 
 
 _import_structure = {
-    "_llm": ["LLM", "Runner"],
+    "_llm": ["LLM", "Runner", "LLMRunner"],
     "_configuration": ["LLMConfig"],
     "_package": ["build"],
     "exceptions": [],
     "_schema": ["GenerationInput", "GenerationOutput", "MetadataOutput"],
     "utils": [],
     "models": [],
     "client": [],
@@ -141,14 +141,15 @@
     from . import client as client
     from . import exceptions as exceptions
     from . import models as models
 
     # Specific types import
     from ._configuration import LLMConfig as LLMConfig
     from ._llm import LLM as LLM
+    from ._llm import LLMRunner as LLMRunner
     from ._llm import Runner as Runner
     from ._package import build as build
     from ._schema import GenerationInput as GenerationInput
     from ._schema import GenerationOutput as GenerationOutput
     from ._schema import MetadataOutput as MetadataOutput
     from .cli import start as start
     from .cli import start_grpc as start_grpc
```

### Comparing `openllm-0.1.2/src/openllm/__main__.py` & `openllm-0.1.3/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/_configuration.py` & `openllm-0.1.3/src/openllm/_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 import orjson
 from cattr.gen import make_dict_unstructure_fn, override
 from deepmerge.merger import Merger
 
 import openllm
 
 from .exceptions import ForbiddenAttributeError, GpuNotAvailableError, OpenLLMException
-from .utils import DEBUG, LazyType, bentoml_cattr, dantic, first_not_none, lenient_issubclass
+from .utils import DEBUG, LazyType, bentoml_cattr, codegen, dantic, first_not_none, lenient_issubclass
 
 if hasattr(t, "Required"):
     from typing import Required
 else:
     from typing_extensions import Required
 
 if hasattr(t, "NotRequired"):
@@ -81,15 +81,15 @@
 _T = t.TypeVar("_T")
 
 
 if t.TYPE_CHECKING:
     import tensorflow as tf
     import torch
     import transformers
-    from attr import _CountingAttr, _make_init, _make_method, _make_repr, _transform_attrs
+    from attr import _CountingAttr, _make_init, _make_repr, _transform_attrs  # type: ignore
     from transformers.generation.beam_constraints import Constraint
 
     from ._types import ClickFunctionWrapper, F, O_co, P
 
     ReprArgs: t.TypeAlias = t.Iterable[tuple[str | None, t.Any]]
 
     DictStrAny = dict[str, t.Any]
@@ -99,15 +99,15 @@
 else:
     Constraint = t.Any
     ListStr = list
     DictStrAny = dict
     ItemgetterAny = itemgetter
     # NOTE: Using internal API from attr here, since we are actually
     # allowing subclass of openllm.LLMConfig to become 'attrs'-ish
-    from attr._make import _CountingAttr, _make_init, _make_method, _make_repr, _transform_attrs
+    from attr._make import _CountingAttr, _make_init, _make_repr, _transform_attrs
 
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     tf = openllm.utils.LazyLoader("tf", globals(), "tensorflow")
 
 __all__ = ["LLMConfig"]
 
@@ -385,97 +385,18 @@
 ) -> t.Any:
     if transform is not None and callable(transform):
         key = transform(key)
 
     return os.environ.get(key, fallback)
 
 
-# sentinel object for unequivocal object() getattr
-_sentinel = object()
-
-
 def _field_env_key(model_name: str, key: str, suffix: str | None = None) -> str:
     return "_".join(filter(None, map(str.upper, ["OPENLLM", model_name, suffix.strip("_") if suffix else "", key])))
 
 
-def _has_own_attribute(cls: type[t.Any], attrib_name: t.Any):
-    """
-    Check whether *cls* defines *attrib_name* (and doesn't just inherit it).
-    """
-    attr = getattr(cls, attrib_name, _sentinel)
-    if attr is _sentinel:
-        return False
-
-    for base_cls in cls.__mro__[1:]:
-        a = getattr(base_cls, attrib_name, None)
-        if attr is a:
-            return False
-
-    return True
-
-
-def _get_annotations(cls: type[t.Any]) -> DictStrAny:
-    """
-    Get annotations for *cls*.
-    """
-    if _has_own_attribute(cls, "__annotations__"):
-        return cls.__annotations__
-
-    return DictStrAny()
-
-
-_classvar_prefixes = (
-    "typing.ClassVar",
-    "t.ClassVar",
-    "ClassVar",
-    "typing_extensions.ClassVar",
-)
-
-
-def _is_class_var(annot: str | t.Any) -> bool:
-    """
-    Check whether *annot* is a typing.ClassVar.
-
-    The string comparison hack is used to avoid evaluating all string
-    annotations which would put attrs-based classes at a performance
-    disadvantage compared to plain old classes.
-    """
-    annot = str(annot)
-
-    # Annotation can be quoted.
-    if annot.startswith(("'", '"')) and annot.endswith(("'", '"')):
-        annot = annot[1:-1]
-
-    return annot.startswith(_classvar_prefixes)
-
-
-def _add_method_dunders(cls: type[t.Any], method_or_cls: _T, _overwrite_doc: str | None = None) -> _T:
-    """
-    Add __module__ and __qualname__ to a *method* if possible.
-    """
-    try:
-        method_or_cls.__module__ = cls.__module__
-    except AttributeError:
-        pass
-
-    try:
-        method_or_cls.__qualname__ = ".".join((cls.__qualname__, method_or_cls.__name__))
-    except AttributeError:
-        pass
-
-    try:
-        method_or_cls.__doc__ = (
-            _overwrite_doc or "Method or class generated by LLMConfig for class " f"{cls.__qualname__}."
-        )
-    except AttributeError:
-        pass
-
-    return method_or_cls
-
-
 # cached it here to save one lookup per assignment
 _object_getattribute = object.__getattribute__
 
 
 class ModelSettings(t.TypedDict, total=False):
     """ModelSettings serve only for typing purposes as this is transcribed into LLMConfig.__config__.
     Note that all fields from this dictionary will then be converted to __openllm_*__ fields in LLMConfig.
@@ -502,16 +423,16 @@
     timeout: int
     workers_per_resource: t.Union[int, float]
 
     # the target generation_config class to be used.
     generation_class: t.Type[GenerationConfig]
 
 
-_ModelSettings: type[attr.AttrsInstance] = _add_method_dunders(
-    type("__internal__", (ModelSettings,), {"__module__": "openllm._configuration"}),
+_ModelSettings: type[attr.AttrsInstance] = codegen.add_method_dunders(
+    type("__openllm_internal__", (ModelSettings,), {"__module__": "openllm._configuration"}),
     attr.make_class(
         "ModelSettings",
         {
             k: dantic.Field(
                 kw_only=False if t.get_origin(ann) is not Required else True,
                 auto_default=True,
                 use_default_converter=False,
@@ -559,62 +480,56 @@
     _cl_name = cl_.__name__.replace("Config", "")
     name_type = first_not_none(settings.get("name_type"), "dasherize")
     model_name = inflection.underscore(_cl_name) if name_type == "dasherize" else _cl_name.lower()
     start_name = inflection.dasherize(model_name) if name_type == "dasherize" else model_name
     partialed = functools.partial(_field_env_key, model_name=model_name, suffix="generation")
 
     def auto_env_transformers(_: t.Any, fields: list[attr.Attribute[t.Any]]) -> list[attr.Attribute[t.Any]]:
-        _has_own_gen = _has_own_attribute(cl_, "GenerationConfig")
+        _has_own_gen = codegen.has_own_attribute(cl_, "GenerationConfig")
         return [
             f.evolve(
                 default=_populate_value_from_env_var(
                     partialed(key=f.name),
                     fallback=getattr(cl_.GenerationConfig, f.name, f.default) if _has_own_gen else f.default,
                 ),
                 metadata={"env": partialed(key=f.name), "description": f.metadata.get("description", "(not provided)")},
                 converter=None,
             )
             for f in fields
         ]
 
-    _target: DictStrAny = {
-        "default_id": settings["default_id"],
-        "model_ids": settings["model_ids"],
-        "url": settings.get("url", ""),
-        "requires_gpu": settings.get("requires_gpu", False),
-        "trust_remote_code": settings.get("trust_remote_code", False),
-        "requirements": settings.get("requirements", None),
-        "name_type": name_type,
-        "model_name": model_name,
-        "start_name": start_name,
-        "env": openllm.utils.ModelEnv(model_name),
-        "timeout": settings.get("timeout", 3600),
-        "workers_per_resource": settings.get("workers_per_resource", 1),
-        "generation_class": attr.make_class(
+    return cls(
+        default_id=settings["default_id"],
+        model_ids=settings["model_ids"],
+        url=settings.get("url", ""),
+        requires_gpu=settings.get("requires_gpu", False),
+        trust_remote_code=settings.get("trust_remote_code", False),
+        requirements=settings.get("requirements", None),
+        name_type=name_type,
+        model_name=model_name,
+        start_name=start_name,
+        env=openllm.utils.ModelEnv(model_name),
+        timeout=settings.get("timeout", 3600),
+        workers_per_resource=settings.get("workers_per_resource", 1),
+        generation_class=attr.make_class(
             f"{_cl_name}GenerationConfig",
             [],
             bases=(GenerationConfig,),
             slots=True,
             weakref_slot=True,
             frozen=False,
             repr=True,
             field_transformer=auto_env_transformers,
         ),
-    }
-
-    return cls(**_target)
+    )
 
 
 bentoml_cattr.register_structure_hook(_ModelSettings, structure_settings)
 
 
-def _generate_unique_filename(cls: type[t.Any], func_name: str):
-    return f"<LLMConfig generated {func_name} {cls.__module__}." f"{getattr(cls, '__qualname__', cls.__name__)}>"
-
-
 def _setattr_class(attr_name: str, value_var: t.Any, add_dunder: bool = False):
     """
     Use the builtin setattr to set *attr_name* to *value_var*.
     We can't use the cached object.__setattr__ since we are setting
     attributes to a class.
     """
     if add_dunder:
@@ -628,38 +543,28 @@
 def _make_assignment_script(cls: type[LLMConfig], attributes: attr.AttrsInstance) -> t.Callable[..., None]:
     """Generate the assignment script with prefix attributes __openllm_<value>__"""
     args: ListStr = []
     globs: DictStrAny = {
         "cls": cls,
         "_cached_attribute": attributes,
         "_cached_getattribute_get": _object_getattribute.__get__,
-        "__add_dunder": _add_method_dunders,
+        "__add_dunder": codegen.add_method_dunders,
     }
     annotations: DictStrAny = {"return": None}
 
     lines: ListStr = ["_getattr = _cached_getattribute_get(_cached_attribute)"]
     for attr_name, field in attr.fields_dict(attributes.__class__).items():
         arg_name = field.metadata.get("target", f"__openllm_{inflection.underscore(attr_name)}__")
         args.append(f"{attr_name}=getattr(_cached_attribute, '{attr_name}')")
         lines.append(_setattr_class(arg_name, attr_name, add_dunder=attr_name in _dunder_add))
         annotations[attr_name] = field.type
 
-    script = "def __assign_attr(cls, %s):\n    %s\n" % (", ".join(args), "\n    ".join(lines) if lines else "pass")
-    assign_method = _make_method(
-        "__assign_attr",
-        script,
-        _generate_unique_filename(cls, "__assign_attr"),
-        globs,
+    return codegen.generate_function(
+        cls, "__assign_attr", lines, args=("cls", *args), globs=globs, annotations=annotations
     )
-    assign_method.__annotations__ = annotations
-
-    if DEBUG:
-        logger.info("Generated script:\n%s", script)
-
-    return assign_method
 
 
 _reserved_namespace = {"__config__", "GenerationConfig"}
 
 
 @attr.define(slots=True)
 class LLMConfig:
@@ -837,15 +742,15 @@
             logger.warning("LLMConfig subclass should end with 'Config'. Updating to %sConfig", cls.__name__)
             cls.__name__ = f"{cls.__name__}Config"
 
         # NOTE: auto assignment attributes generated from __config__
         _make_assignment_script(cls, bentoml_cattr.structure(cls, _ModelSettings))(cls)
         # process a fields under cls.__dict__ and auto convert them with dantic.Field
         cd = cls.__dict__
-        anns = _get_annotations(cls)
+        anns = codegen.get_annotations(cls)
         partialed = functools.partial(_field_env_key, model_name=cls.__openllm_model_name__)
 
         def auto_config_env(_: type[LLMConfig], attrs: list[attr.Attribute[t.Any]]) -> list[attr.Attribute[t.Any]]:
             return [
                 a.evolve(
                     default=_populate_value_from_env_var(partialed(key=a.name), fallback=a.default),
                     metadata={
@@ -857,15 +762,15 @@
             ]
 
         # _CountingAttr is the underlying representation of attr.field
         ca_names = {name for name, attr in cd.items() if isinstance(attr, _CountingAttr)}
         these: dict[str, _CountingAttr[t.Any]] = {}
         annotated_names: set[str] = set()
         for attr_name, typ in anns.items():
-            if _is_class_var(typ):
+            if codegen.is_class_var(typ):
                 continue
             annotated_names.add(attr_name)
             val = cd.get(attr_name, attr.NOTHING)
             if not LazyType["_CountingAttr[t.Any]"](_CountingAttr).isinstance(val):
                 if val is attr.NOTHING:
                     val = cls.Field(env=partialed(key=attr_name))
                 else:
@@ -903,15 +808,15 @@
         _attr_names = tuple(a.name for a in attrs)
         _has_pre_init = bool(getattr(cls, "__attrs_pre_init__", False))
         _has_post_init = bool(getattr(cls, "__attrs_post_init__", False))
         # the protocol for attrs-decorated class
         cls.__attrs_attrs__ = attrs
         # generate a __attrs_init__ for the subclass, since we will
         # implement a custom __init__
-        cls.__attrs_init__ = _add_method_dunders(
+        cls.__attrs_init__ = codegen.add_method_dunders(
             cls,
             _make_init(
                 cls,  # cls (the attrs-decorated class)
                 attrs,  # tuple of attr.Attribute of cls
                 _has_pre_init,  # pre_initjk
                 _has_post_init,  # post_init
                 False,  # frozen
@@ -920,15 +825,15 @@
                 base_attr_map,  # base_attr_map
                 False,  # is_exc (check if it is exception)
                 None,  # cls_on_setattr (essentially attr.setters)
                 attrs_init=True,  # whether to create __attrs_init__ instead of __init__
             ),
         )
         # __repr__ function with the updated fields.
-        cls.__repr__ = _add_method_dunders(cls, _make_repr(cls.__attrs_attrs__, None, cls))
+        cls.__repr__ = codegen.add_method_dunders(cls, _make_repr(cls.__attrs_attrs__, None, cls))
         # Traverse the MRO to collect existing slots
         # and check for an existing __weakref__.
         existing_slots: DictStrAny = dict()
         weakref_inherited = False
         for base_cls in cls.__mro__[1:-1]:
             if base_cls.__dict__.get("__weakref__", None) is not None:
                 weakref_inherited = True
```

### Comparing `openllm-0.1.2/src/openllm/_llm.py` & `openllm-0.1.3/src/openllm/_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,28 @@
 from __future__ import annotations
 
 import copy
 import functools
 import logging
 import os
 import re
-import sys
 import types
 import typing as t
-from abc import ABC, ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
 
+import attr
 import bentoml
 import inflection
 import orjson
 from bentoml._internal.models.model import ModelSignature
 from bentoml._internal.types import ModelSignatureDict
 
 import openllm
 
 from .exceptions import ForbiddenAttributeError, OpenLLMException
-from .models.auto import AutoConfig
 from .utils import ENV_VARS_TRUE_VALUES, LazyLoader, bentoml_cattr
 
 if t.TYPE_CHECKING:
     import torch
     import transformers
     from bentoml._internal.runner.strategy import Strategy
 
@@ -47,26 +46,29 @@
         llm_type: str
         identifying_params: dict[str, t.Any]
 
         def __call__(self, *args: t.Any, **attrs: t.Any) -> t.Any:
             ...
 
 else:
+    LLMRunner = bentoml.Runner
     transformers = LazyLoader("transformers", globals(), "transformers")
     torch = LazyLoader("torch", globals(), "torch")
 
 logger = logging.getLogger(__name__)
 
 # NOTE: `1-2` -> text-generation and text2text-generation
 FRAMEWORK_TO_AUTOCLASS_MAPPING = {
     "pt": ("AutoModelForCausalLM", "AutoModelForSeq2SeqLM"),
     "tf": ("TFAutoModelForCausalLM", "TFAutoModelForSeq2SeqLM"),
     "flax": ("FlaxAutoModelForCausalLM", "FlaxAutoModelForSeq2SeqLM"),
 }
 
+TOKENIZER_PREFIX = "_tokenizer_"
+
 
 def convert_transformers_model_name(name: str) -> str:
     if os.path.exists(os.path.dirname(name)):
         name = os.path.basename(name)
         logger.debug("Given name is a path, only returning the basename %s")
         return name
     return re.sub("[^a-zA-Z0-9]+", "-", name)
@@ -173,17 +175,20 @@
 class LLMInterface(ABC):
     """This defines the loose contract for all openllm.LLM implementations."""
 
     config_class: type[openllm.LLMConfig]
     """The config class to use for this LLM. If you are creating a custom LLM, you must specify this class."""
 
     @property
-    def import_kwargs(self) -> dict[str, t.Any] | None:
+    def import_kwargs(self) -> tuple[dict[str, t.Any], dict[str, t.Any]] | None:
         """The default import kwargs to used when importing the model.
-        This will be passed into 'openllm.LLM.import_model'."""
+        This will be passed into 'openllm.LLM.import_model'.
+        It returns two dictionaries: one for model kwargs and one for tokenizer kwargs.
+        """
+        return
 
     @abstractmethod
     def generate(self, prompt: str, **preprocess_generate_kwds: t.Any) -> t.Any:
         """The main function implementation for generating from given prompt.  It takes the prompt
         and the generation_kwargs from 'self.sanitize_parameters' and then
         pass it to 'self.model.generate'.
         """
@@ -249,140 +254,95 @@
         self.load_in_mha = False
 
 
 _M = t.TypeVar("_M")
 _T = t.TypeVar("_T")
 
 
-class LLMMetaclass(ABCMeta):
-    def __new__(
-        mcls, cls_name: str, bases: tuple[type[t.Any], ...], namespace: dict[str, t.Any], **attrs: t.Any
-    ) -> type:
-        """Metaclass for creating a LLM."""
-        if LLMInterface not in bases:  # only actual openllm.LLM should hit this branch.
-            annotations_dict: dict[str, t.Any] = {}
-
-            # NOTE: set implementation branch
-            prefix_class_name_config = cls_name
-            if cls_name.startswith("Flax"):
-                implementation = "flax"
-                prefix_class_name_config = cls_name[4:]
-                annotations_dict.update(
-                    {
-                        "__llm_model__": "transformers.FlaxPreTrainedModel",
-                        "model": "transformers.FlaxPreTrainedModel",
-                    }
-                )
-            elif cls_name.startswith("TF"):
-                implementation = "tf"
-                prefix_class_name_config = cls_name[2:]
-                annotations_dict.update(
-                    {
-                        "__llm_model__": "transformers.TFPreTrainedModel",
-                        "model": "transformers.TFPreTrainedModel",
-                    }
-                )
-            else:
-                implementation = "pt"
-                annotations_dict.update(
-                    {
-                        "__llm_model__": "transformers.PreTrainedModel",
-                        "model": "transformers.PreTrainedModel",
-                    }
-                )
-            namespace["__llm_implementation__"] = implementation
-
-            config_class = AutoConfig.infer_class_from_name(prefix_class_name_config)
-            annotations_dict["config_class"] = f"type[openllm.{config_class.__qualname__}]"
-            annotations_dict["config"] = f"openllm.{config_class.__qualname__}"
-
-            # NOTE: setup config class branch
-            if "__openllm_internal__" in namespace:
-                # NOTE: we will automatically find the subclass for this given config class
-                if "config_class" not in namespace:
-                    # this branch we will automatically get the class
-                    namespace["config_class"] = config_class
-                else:
-                    logger.debug(f"Using config class {namespace['config_class']} for {cls_name}.")
-            # NOTE: check for required attributes
-            else:
-                if "config_class" not in namespace:
-                    raise RuntimeError(
-                        "Missing required key 'config_class'. Make sure to define it within the LLM subclass."
-                    )
-
-            # NOTE: the llm_post_init branch
-            if "llm_post_init" in namespace:
-                original_llm_post_init = namespace["llm_post_init"]
-
-                def wrapped_llm_post_init(self: LLM[t.Any, t.Any]) -> None:
-                    """We need to both initialize private attributes and call the user-defined model_post_init
-                    method.
-                    """
-                    _default_post_init(self)
-                    original_llm_post_init(self)
+@attr.define(slots=True, repr=False)
+class LLM(LLMInterface, t.Generic[_M, _T]):
+    if t.TYPE_CHECKING:
+        # The following will be populated by metaclass
+        __llm_trust_remote_code__: bool
+        __llm_implementation__: t.Literal["pt", "tf", "flax"]
+        __llm_model__: _M | None
+        __llm_tokenizer__: _T | None
+        __llm_tag__: bentoml.Tag | None
+        __llm_bentomodel__: bentoml.Model | None
 
-                namespace["llm_post_init"] = wrapped_llm_post_init
-            else:
-                namespace["llm_post_init"] = _default_post_init
+        __openllm_post_init__: t.Callable[[t.Self], None] | None
+        __openllm_custom_load__: t.Callable[[t.Self, t.Any, t.Any], None] | None
+        __openllm_custom_import_kwargs__: property | None
 
-            # NOTE: import_model branch
-            if "import_model" not in namespace:
-                # using the default import model
-                namespace["import_model"] = functools.partial(import_model, _model_framework=implementation)
+        _model_args: tuple[t.Any, ...]
+        _model_attrs: dict[str, t.Any]
+        _tokenizer_attrs: dict[str, t.Any]
+
+    def __init_subclass__(cls):
+        cd = cls.__dict__
+        prefix_class_name_config = cls.__name__
+        if prefix_class_name_config.startswith("Flax"):
+            implementation = "flax"
+            prefix_class_name_config = prefix_class_name_config[4:]
+        elif prefix_class_name_config.startswith("TF"):
+            implementation = "tf"
+            prefix_class_name_config = prefix_class_name_config[2:]
+        else:
+            implementation = "pt"
+        cls.__llm_implementation__ = implementation
+        config_class = openllm.AutoConfig.infer_class_from_name(prefix_class_name_config)
+
+        if "__openllm_internal__" in cd:
+            if "config_class" not in cd:
+                cls.config_class = config_class
             else:
-                logger.debug("Using custom 'import_model' for %s", cls_name)
-
-            namespace.update({k: None for k in {"__llm_model__", "__llm_tokenizer__", "__llm_bentomodel__"}})
-            tokenizer_type = "typing.Optional[transformers.PreTrainedTokenizerFast]"
-            annotations_dict.update(
-                {
-                    "load_in_mha": "bool",
-                    "tokenizer": tokenizer_type,
-                    "__llm_tokenizer__": tokenizer_type,
-                    "__llm_bentomodel__": "typing.Optional[bentoml.Model]",
-                }
-            )
-            # NOTE: transformers to ForwardRef
-            for key, value in annotations_dict.items():
-                if (3, 10) > sys.version_info >= (3, 9, 8) or sys.version_info >= (3, 10, 1):
-                    annotations_dict[key] = t.ForwardRef(value, is_argument=False, is_class=True)
-                else:
-                    annotations_dict[key] = t.ForwardRef(value, is_argument=False)
+                logger.debug(f"Using config class {cd['config_class']} for {cls.__name__}.")
+        else:
+            if "config_class" not in cd:
+                raise RuntimeError(
+                    "Missing required key 'config_class'. Make sure to define it within the LLM subclass."
+                )
 
-            namespace["__annotations__"] = annotations_dict
+        if cls.llm_post_init is not LLMInterface.llm_post_init:
+            original_llm_post_init = cd["llm_post_init"]
 
-            cls: type[LLM[t.Any, t.Any]] = super().__new__(
-                t.cast("type[type[LLM[t.Any, t.Any]]]", mcls), cls_name, bases, namespace, **attrs
-            )
+            def wrapped_llm_post_init(self: t.Self) -> None:
+                """We need to both initialize private attributes and call the user-defined model_post_init
+                method.
+                """
+                _default_post_init(self)
+                original_llm_post_init(self)
 
-            cls.__openllm_post_init__ = None if cls.llm_post_init is LLMInterface.llm_post_init else cls.llm_post_init
-            cls.__openllm_custom_load__ = None if cls.load_model is LLMInterface.load_model else cls.load_model
-            return cls
+            cls.llm_post_init = wrapped_llm_post_init
         else:
-            # the LLM class itself being created, no need to setup
-            return super().__new__(mcls, cls_name, bases, namespace, **attrs)
-
+            setattr(cls, "llm_post_init", _default_post_init)
 
-class LLM(LLMInterface, t.Generic[_M, _T], metaclass=LLMMetaclass):
-    if t.TYPE_CHECKING:
-        # NOTE: the following will be populated by metaclass
-        __llm_implementation__: t.Literal["pt", "tf", "flax"]
+        if cls.import_model is LLMInterface.import_model:
+            # using the default import model
+            setattr(cls, "import_model", functools.partial(import_model, _model_framework=implementation))
+        else:
+            logger.debug("Using custom 'import_model' for %s", cls.__name__)
 
-        __openllm_post_init__: t.Callable[[t.Self], None] | None
-        __openllm_custom_load__: t.Callable[[t.Self, t.Any, t.Any], None] | None
+        cls.__openllm_post_init__ = None if cls.llm_post_init is LLMInterface.llm_post_init else cls.llm_post_init
+        cls.__openllm_custom_load__ = None if cls.load_model is LLMInterface.load_model else cls.load_model
+        cls.__openllm_custom_import_kwargs__ = (
+            None if cls.import_kwargs is LLMInterface.import_kwargs else cls.import_kwargs
+        )
 
-        load_in_mha: bool
-        _llm_attrs: dict[str, t.Any]
-        _llm_args: tuple[t.Any, ...]
+        for at in {"bentomodel", "tag", "model", "tokenizer"}:
+            setattr(cls, f"__llm_{at}__", None)
 
-    # NOTE: the following is the similar interface to HuggingFace pretrained protocol.
+    # The following is the similar interface to HuggingFace pretrained protocol.
     @classmethod
     def from_pretrained(
-        cls, model_id: str | None = None, llm_config: openllm.LLMConfig | None = None, *args: t.Any, **attrs: t.Any
+        cls,
+        model_id: str | None = None,
+        llm_config: openllm.LLMConfig | None = None,
+        *args: t.Any,
+        **attrs: t.Any,
     ) -> LLM[_M, _T]:
         return cls(model_id=model_id, llm_config=llm_config, *args, **attrs)
 
     def __init__(
         self,
         model_id: str | None = None,
         llm_config: openllm.LLMConfig | None = None,
@@ -469,14 +429,15 @@
         The following are optional:
             openllm_model_version: version for this `model_id`. By default, users can ignore this if using pretrained
                                    weights as OpenLLM will use the commit_hash of given model_id.
                                    However, if `model_id` is a path, this argument is recomended to include.
         """
 
         load_in_mha = attrs.pop("load_in_mha", False)
+        openllm_model_version = attrs.pop("openllm_model_version", None)
 
         if llm_config is not None:
             logger.debug("Using given 'llm_config=(%s)' to initialize LLM", llm_config)
             self.config = llm_config
         else:
             self.config = self.config_class(**attrs)
             # The rests of the kwargs that is not used by the config class should be stored into __openllm_extras__.
@@ -485,225 +446,179 @@
         if model_id is None:
             model_id = os.environ.get(self.config.__openllm_env__.model_id, self.config.__openllm_default_id__)
             assert model_id is not None
 
         # NOTE: This is the actual given path or pretrained weight for this LLM.
         self._model_id = model_id
 
+        # parsing tokenizer and model kwargs
+        tokenizer_kwds = {k[len(TOKENIZER_PREFIX) :]: v for k, v in attrs.items() if k.startswith(TOKENIZER_PREFIX)}
+        for k in attrs:
+            if k in tokenizer_kwds:
+                del attrs[k]
+        # the rest of kwargs should be model kwargs
+        model_kwds = attrs
+
+        if self.import_kwargs:
+            _custom_model_kwds, _custom_tokenizer_kwds = self.import_kwargs
+            model_kwds.update(_custom_model_kwds)
+            tokenizer_kwds.update(_custom_tokenizer_kwds)
+
+        # handle trust_remote_code
+        self.__llm_trust_remote_code__ = model_kwds.pop("trust_remote_code", self.config.__openllm_trust_remote_code__)
+
         # NOTE: Save the args and kwargs for latter load
-        self._llm_args = args
-        self._llm_attrs = attrs
+        self._model_args = args
+        self._model_attrs = model_kwds
+        self._tokenizer_attrs = tokenizer_kwds
 
         if self.__openllm_post_init__:
             self.llm_post_init()
 
         # finally: we allow users to overwrite the load_in_mha defined by the LLM subclass.
         if load_in_mha:
+            logger.debug("Overwriting 'load_in_mha=%s' (base load_in_mha=%s)", load_in_mha, self.load_in_mha)
             self.load_in_mha = load_in_mha
 
+        self._openllm_model_version = openllm_model_version
+
     def __setattr__(self, attr: str, value: t.Any):
         if attr in _reserved_namespace:
             raise ForbiddenAttributeError(
                 f"{attr} should not be set during runtime "
                 f"as these value will be reflected during runtime. "
                 f"Instead, you can create a custom LLM subclass {self.__class__.__name__}."
             )
 
         super().__setattr__(attr, value)
 
+    def __repr__(self) -> str:
+        keys = {"model_id", "runner_name", "llm_type", "config"}
+        return f"{self.__class__.__name__}({', '.join(f'{k}={getattr(self, k)!r}' for k in keys)})"
+
     @property
     def model_id(self) -> str:
         return self._model_id
 
+    @property
+    def runner_name(self) -> str:
+        return f"llm-{self.config.__openllm_start_name__}-runner"
+
     # NOTE: The section below defines a loose contract with langchain's LLM interface.
     @property
     def llm_type(self) -> str:
         return convert_transformers_model_name(self._model_id)
 
     @property
     def identifying_params(self) -> dict[str, t.Any]:
         return {
             "configuration": self.config.model_dump_json().decode(),
             "model_ids": orjson.dumps(self.config.__openllm_model_ids__).decode(),
         }
 
-    @t.overload
-    def make_tag(
-        self,
-        model_id: str | None = None,
-        return_unused_kwargs: t.Literal[False] = ...,
-        trust_remote_code: bool = ...,
-        **attrs: t.Any,
-    ) -> bentoml.Tag:
-        ...
-
-    @t.overload
-    def make_tag(
-        self,
-        model_id: str | None = None,
-        return_unused_kwargs: t.Literal[True] = ...,
-        trust_remote_code: bool = ...,
-        **attrs: t.Any,
-    ) -> tuple[bentoml.Tag, dict[str, t.Any]]:
-        ...
-
-    def make_tag(
-        self,
-        model_id: str | None = None,
-        return_unused_kwargs: bool = False,
-        trust_remote_code: bool = False,
-        **attrs: t.Any,
-    ) -> bentoml.Tag | tuple[bentoml.Tag, dict[str, t.Any]]:
+    def make_tag(self, model_id: str | None = None) -> bentoml.Tag:
         """Generate a ``bentoml.Tag`` from a given transformers model name.
 
         Note that this depends on your model to have a config class available.
 
         Args:
-            model_name_or_path: The transformers model name or path to load the model from.
-                                If it is a path, then `openllm_model_version` must be passed in as a kwarg.
-            return_unused_kwargs: Whether to return unused kwargs. Defaults to False. If set, it will return a tuple
-                                  of ``bentoml.Tag`` and a dict of unused kwargs.
+            model_id: The transformers model name or path to load the model from.
+                      If it is a path, then `openllm_model_version` must be passed in as a kwarg.
             trust_remote_code: Whether to trust the remote code. Defaults to False.
             **attrs: Additional kwargs to pass to the ``transformers.AutoConfig`` constructor.
                     If your pass ``return_unused_kwargs=True``, it will be ignored.
 
         Returns:
             A tuple of ``bentoml.Tag`` and a dict of unused kwargs.
         """
         if model_id is None:
             model_id = self._model_id
-
-        if "return_unused_kwargs" in attrs:
-            logger.debug("Ignoring 'return_unused_kwargs' in 'generate_tag_from_model_name'.")
-            attrs.pop("return_unused_kwargs", None)
-
-        config, attrs = t.cast(
-            "tuple[transformers.PretrainedConfig, dict[str, t.Any]]",
-            transformers.AutoConfig.from_pretrained(
-                model_id, return_unused_kwargs=True, trust_remote_code=trust_remote_code, **attrs
-            ),
-        )
         name = convert_transformers_model_name(model_id)
 
-        if os.path.exists(os.path.dirname(model_id)):
-            # If the model_name_or_path is a path, we assume it's a local path,
-            # then users must pass a version for this.
-            model_version = attrs.pop("openllm_model_version", None)
-            if model_version is None:
-                logger.warning(
-                    """\
-            When passing a path, it is recommended to also pass 'openllm_model_version'
-            into Runner/AutoLLM intialization.
-
-            For example:
-
-            >>> import openllm
-            >>> runner = openllm.Runner('/path/to/fine-tuning/model', openllm_model_version='lora-version')
-
-            Example with AutoLLM:
-
-            >>> import openllm
-            >>> model = openllm.AutoLLM.for_model('/path/to/fine-tuning/model', openllm_model_version='lora-version')
+        config = t.cast(
+            "transformers.PretrainedConfig",
+            transformers.AutoConfig.from_pretrained(model_id, trust_remote_code=self.__llm_trust_remote_code__),
+        )
 
-            No worries, OpenLLM will generate one for you. But for your own convenience, make sure to
-            specify 'openllm_model_version'.
-            """
-                )
-                model_version = bentoml.Tag.from_taglike(name).make_new_version().version
-        else:
-            model_version = getattr(config, "_commit_hash", None)
-            if model_version is None:
+        model_version = getattr(config, "_commit_hash", None)
+        if model_version is None:
+            if self._openllm_model_version is not None:
                 logger.warning(
-                    "Given %s from '%s' doesn't contain a commit hash. We will generate"
-                    " the tag without specific version.",
-                    t.cast("type[transformers.PretrainedConfig]", config.__class__),
+                    "Given %s from '%s' doesn't contain a commit hash, and 'openllm_model_version' is not given. "
+                    "We will generate the tag without specific version.",
+                    config.__class__,
                     model_id,
                 )
-        tag = bentoml.Tag.from_taglike(f"{self.__llm_implementation__}-{name}:{model_version}")
+                model_version = bentoml.Tag.from_taglike(name).make_new_version().version
+            else:
+                logger.debug("Using %s for '%s' as model version", self._openllm_model_version, model_id)
+                model_version = self._openllm_model_version
 
-        if return_unused_kwargs:
-            return tag, attrs
-        return tag
+        return bentoml.Tag.from_taglike(f"{self.__llm_implementation__}-{name}:{model_version}")
 
     def ensure_model_id_exists(self) -> bentoml.Model:
-        trust_remote_code = self._llm_attrs.pop("trust_remote_code", self.config.__openllm_trust_remote_code__)
-        tag, kwds = self.make_tag(return_unused_kwargs=True, trust_remote_code=trust_remote_code, **self._llm_attrs)
         try:
-            return bentoml.transformers.get(tag)
-        except bentoml.exceptions.BentoMLException:
-            logger.info("'%s' with tag (%s) not found, importing from HuggingFace Hub.", self.__class__.__name__, tag)
-            tokenizer_kwds = {k[len("_tokenizer_") :]: v for k, v in kwds.items() if k.startswith("_tokenizer_")}
-            kwds = {k: v for k, v in kwds.items() if not k.startswith("_tokenizer_")}
-
-            if self.import_kwargs:
-                tokenizer_kwds = {
-                    **{
-                        k[len("_tokenizer_") :]: v for k, v in self.import_kwargs.items() if k.startswith("_tokenizer_")
-                    },
-                    **tokenizer_kwds,
-                }
-                kwds = {
-                    **{k: v for k, v in self.import_kwargs.items() if not k.startswith("_tokenizer_")},
-                    **kwds,
-                }
-
+            return bentoml.transformers.get(self.tag)
+        except bentoml.exceptions.NotFound:
+            logger.info(
+                "'%s' with tag (%s) not found, importing from HuggingFace Hub.", self.__class__.__name__, self.tag
+            )
             return self.import_model(
                 self._model_id,
-                tag,
-                *self._llm_args,
-                tokenizer_kwds=tokenizer_kwds,
-                trust_remote_code=trust_remote_code,
-                **kwds,
+                self.tag,
+                *self._model_args,
+                tokenizer_kwds=self._tokenizer_attrs,
+                trust_remote_code=self.__llm_trust_remote_code__,
+                **self._model_attrs,
             )
         finally:
             if openllm.utils.is_torch_available() and torch.cuda.is_available():
                 torch.cuda.empty_cache()
 
     @property
     def _bentomodel(self) -> bentoml.Model:
         if self.__llm_bentomodel__ is None:
             self.__llm_bentomodel__ = self.ensure_model_id_exists()
         return self.__llm_bentomodel__
 
     @property
     def tag(self) -> bentoml.Tag:
-        return self._bentomodel.tag
+        if self.__llm_tag__ is None:
+            self.__llm_tag__ = self.make_tag()
+        return self.__llm_tag__
 
     @property
     def model(self) -> _M:
         """The model to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
         # Run check for GPU
-        trust_remote_code = self._llm_attrs.pop("trust_remote_code", self.config.__openllm_trust_remote_code__)
         self.config.check_if_gpu_is_available(implementation=self.__llm_implementation__)
 
-        kwds = {k: v for k, v in self._llm_attrs.items() if not k.startswith("_tokenizer_")}
-
-        if self.import_kwargs:
-            kwds = {**{k: v for k, v in self.import_kwargs.items() if not k.startswith("_tokenizer_")}, **kwds}
+        kwds = self._model_attrs
+        kwds["trust_remote_code"] = self.__llm_trust_remote_code__
 
-        kwds["trust_remote_code"] = trust_remote_code
         if self.load_in_mha and "_pretrained_class" not in self._bentomodel.info.metadata:
             # This is a pipeline, provide a accelerator args
             kwds["accelerator"] = "bettertransformer"
 
         if self.__llm_model__ is None:
             if self.__openllm_custom_load__:
-                self.__llm_model__ = self.load_model(self.tag, *self._llm_args, **kwds)
+                self.__llm_model__ = self.load_model(self.tag, *self._model_args, **kwds)
             else:
-                self.__llm_model__ = self._bentomodel.load_model(*self._llm_args, **kwds)
+                self.__llm_model__ = self._bentomodel.load_model(*self._model_args, **kwds)
 
-        if (
-            self.load_in_mha
-            and all(i in self._bentomodel.info.metadata for i in ("_framework", "_pretrained_class"))
-            and self._bentomodel.info.metadata["_framework"] == "torch"
-        ):
-            # BetterTransformer is currently only supported on PyTorch.
-            from optimum.bettertransformer import BetterTransformer
+            # TODO: self.config.__openllm_runtime__: t.Literal['python', 'cpp']
+            if (
+                self.load_in_mha
+                and all(i in self._bentomodel.info.metadata for i in ("_framework", "_pretrained_class"))
+                and self._bentomodel.info.metadata["_framework"] == "torch"
+            ):
+                # BetterTransformer is currently only supported on PyTorch.
+                from optimum.bettertransformer import BetterTransformer
 
-            self.__llm_model__ = BetterTransformer.transform(self.__llm_model__)
+                self.__llm_model__ = BetterTransformer.transform(self.__llm_model__)
         return t.cast(_M, self.__llm_model__)
 
     @property
     def tokenizer(self) -> _T:
         """The tokenizer to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
         if self.__llm_tokenizer__ is None:
             try:
@@ -738,19 +653,15 @@
             embedded: Whether to run this runner in embedded mode.
             scheduling_strategy: Whether to create a custom scheduling strategy for this Runner.
 
         NOTE: There are some difference between bentoml.models.get().to_runner() and LLM.to_runner(): 'name'.
         - 'name': will be generated by OpenLLM, hence users don't shouldn't worry about this.
             The generated name will be 'llm-<model-start-name>-runner' (ex: llm-dolly-v2-runner, llm-chatglm-runner)
         """
-
-        name = f"llm-{self.config.__openllm_start_name__}-runner"
         models = models if models is not None else []
-
-        # NOTE: The side effect of this is that will load the imported model during runner creation.
         models.append(self._bentomodel)
 
         if scheduling_strategy is None:
             from bentoml._internal.runner.strategy import DefaultStrategy
 
             scheduling_strategy = DefaultStrategy
 
@@ -771,14 +682,20 @@
             llm_type: str
             identifying_params: dict[str, t.Any]
 
             def __init_subclass__(cls, llm_type: str, identifying_params: dict[str, t.Any], **_: t.Any):
                 cls.llm_type = llm_type
                 cls.identifying_params = identifying_params
 
+            def __init__(__self: _Runnable):
+                # NOTE: The side effect of this line
+                # is that it will load the imported model during
+                # runner creation. So don't remove it!!
+                self.model
+
             @bentoml.Runnable.method(
                 batchable=generate_sig.batchable,
                 batch_dim=generate_sig.batch_dim,
                 input_spec=generate_sig.input_spec,
                 output_spec=generate_sig.output_spec,
             )
             def __call__(__self, prompt: str, **attrs: t.Any) -> list[t.Any]:
@@ -798,29 +715,25 @@
                 batch_dim=generate_iterator_sig.batch_dim,
                 input_spec=generate_iterator_sig.input_spec,
                 output_spec=generate_iterator_sig.output_spec,
             )
             def generate_iterator(__self, prompt: str, **attrs: t.Any) -> t.Iterator[t.Any]:
                 yield self.generate_iterator(prompt, **attrs)
 
-        def _wrapped_generate_run(__self: bentoml.Runner, *args: t.Any, **kwargs: t.Any) -> t.Any:
+        def _wrapped_generate_run(__self: LLMRunner, prompt: str, **kwargs: t.Any) -> t.Any:
             """Wrapper for runner.generate.run() to handle the prompt and postprocessing.
 
             This will be used for LangChain API.
 
             Usage:
             ```python
             runner = openllm.Runner("dolly-v2", init_local=True)
             runner("What is the meaning of life?")
             ```
             """
-            if len(args) > 1:
-                raise RuntimeError("Only one positional argument is allowed for generate()")
-            prompt = args[0] if len(args) == 1 else kwargs.pop("prompt", "")
-
             prompt, generate_kwargs, postprocess_kwargs = self.sanitize_parameters(prompt, **kwargs)
             generated_result = __self.generate.run(prompt, **generate_kwargs)
             return self.postprocess_generate(prompt, generated_result, **postprocess_kwargs)
 
         # NOTE: returning the two langchain API's to the runner
         return types.new_class(
             inflection.camelize(self.config.__openllm_model_name__) + "Runner",
@@ -844,15 +757,15 @@
                     "SUPPORTED_RESOURCES": ("nvidia.com/gpu", "cpu")
                     if self.config.__openllm_requires_gpu__
                     else ("nvidia.com/gpu",),
                     "llm_type": self.llm_type,
                     "identifying_params": self.identifying_params,
                 },
             ),
-            name=name,
+            name=self.runner_name,
             models=models,
             max_batch_size=max_batch_size,
             max_latency_ms=max_latency_ms,
             method_configs=bentoml_cattr.unstructure(method_configs),
             embedded=embedded,
             scheduling_strategy=scheduling_strategy,
         )
@@ -863,35 +776,68 @@
 
     def __call__(self, prompt: str, **attrs: t.Any) -> t.Any:
         """Returns the generation result and format the result.
 
         First, it runs `self.sanitize_parameters` to sanitize the parameters.
         The the sanitized prompt and kwargs will be pass into self.generate.
         Finally, run self.postprocess_generate to postprocess the generated result.
+
+        This allows users to do the following:
+
+        ```python
+        llm = openllm.AutoLLM.for_model("dolly-v2")
+        llm("What is the meaning of life?")
+        ```
         """
         prompt, generate_kwargs, postprocess_kwargs = self.sanitize_parameters(prompt, **attrs)
         generated_result = self.generate(prompt, **generate_kwargs)
         return self.postprocess_generate(prompt, generated_result, **postprocess_kwargs)
 
 
-def Runner(start_name: str, **attrs: t.Any) -> LLMRunner:
+@t.overload
+def Runner(
+    model_name: str,
+    *,
+    model_id: str | None = None,
+    init_local: t.Literal[False, True] = ...,
+    **attrs: t.Any,
+) -> LLMRunner:
+    ...
+
+
+@t.overload
+def Runner(
+    model_name: str,
+    *,
+    model_id: str = ...,
+    models: list[bentoml.Model] | None = ...,
+    max_batch_size: int | None = ...,
+    max_latency_ms: int | None = ...,
+    method_configs: dict[str, ModelSignatureDict | ModelSignature] | None = ...,
+    embedded: t.Literal[True, False] = ...,
+    scheduling_strategy: type[Strategy] | None = ...,
+    **attrs: t.Any,
+) -> LLMRunner:
+    ...
+
+
+def Runner(model_name: str, **attrs: t.Any) -> LLMRunner:
     """Create a Runner for given LLM. For a list of currently supported LLM, check out 'openllm models'
 
     Args:
-        start_name: Supported model name from 'openllm models'
-        init_local: Whether to init_local this given Runner. This is useful during development. (Default to False)
+        model_name: Supported model name from 'openllm models'
         **attrs: The rest of kwargs will then be passed to the LLM. Refer to the LLM documentation for the kwargs
                 behaviour
     """
     init_local = attrs.pop("init_local", False)
-    ModelEnv = openllm.utils.ModelEnv(start_name)
+    ModelEnv = openllm.utils.ModelEnv(model_name)
     if ModelEnv.get_framework_env() == "flax":
-        runner = openllm.AutoFlaxLLM.create_runner(start_name, **attrs)
+        runner = openllm.AutoFlaxLLM.create_runner(model_name, **attrs)
     elif ModelEnv.get_framework_env() == "tf":
-        runner = openllm.AutoTFLLM.create_runner(start_name, **attrs)
+        runner = openllm.AutoTFLLM.create_runner(model_name, **attrs)
     else:
-        runner = openllm.AutoLLM.create_runner(start_name, **attrs)
+        runner = openllm.AutoLLM.create_runner(model_name, **attrs)
 
     if init_local:
         runner.init_local(quiet=True)
 
     return runner
```

### Comparing `openllm-0.1.2/src/openllm/_package.py` & `openllm-0.1.3/src/openllm/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/_prompt.py` & `openllm-0.1.3/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/_schema.py` & `openllm-0.1.3/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/_service.py` & `openllm-0.1.3/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/_types.py` & `openllm-0.1.3/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/cli.py` & `openllm-0.1.3/src/openllm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -880,32 +880,30 @@
         if env == "flax":
             model = openllm.AutoFlaxLLM.for_model(model_name, model_id=model_id, llm_config=config)
         elif env == "tf":
             model = openllm.AutoTFLLM.for_model(model_name, model_id=model_id, llm_config=config)
         else:
             model = openllm.AutoLLM.for_model(model_name, model_id=model_id, llm_config=config)
 
-        tag = model.make_tag(trust_remote_code=config.__openllm_trust_remote_code__)
-
-        if len(bentoml.models.list(tag)) == 0:
+        if len(bentoml.models.list(model.tag)) == 0:
             if output == "pretty":
-                _echo(f"{tag} does not exists yet!. Downloading...", fg="yellow", nl=True)
+                _echo(f"{model.tag} does not exists yet!. Downloading...", fg="yellow", nl=True)
             m = model.ensure_model_id_exists()
             if output == "pretty":
                 _echo(f"Saved model: {m.tag}")
             elif output == "json":
                 _echo(
                     orjson.dumps(
                         {"previously_setup": False, "framework": env, "tag": str(m.tag)}, option=orjson.OPT_INDENT_2
                     ).decode()
                 )
             else:
-                _echo(tag)
+                _echo(model.tag)
         else:
-            m = bentoml.transformers.get(tag)
+            m = bentoml.transformers.get(model.tag)
             if output == "pretty":
                 _echo(f"{model_name} is already setup for framework '{env}': {str(m.tag)}", nl=True, fg="yellow")
             elif output == "json":
                 _echo(
                     orjson.dumps(
                         {"previously_setup": True, "framework": env, "model": str(m.tag)}, option=orjson.OPT_INDENT_2
                     ).decode(),
```

### Comparing `openllm-0.1.2/src/openllm/client.py` & `openllm-0.1.3/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/exceptions.py` & `openllm-0.1.3/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/__init__.py` & `openllm-0.1.3/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/auto/__init__.py` & `openllm-0.1.3/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/auto/configuration_auto.py` & `openllm-0.1.3/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/auto/factory.py` & `openllm-0.1.3/src/openllm/models/auto/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,19 @@
         """
         runner_kwargs_name = [
             "models",
             "max_batch_size",
             "max_latency_ms",
             "method_configs",
             "embedded",
+            "scheduling_strategy",
         ]
         to_runner_attrs = {k: v for k, v in attrs.items() if k in runner_kwargs_name}
+        for k in to_runner_attrs:
+            del attrs[k]
         if not isinstance(llm_config, openllm.LLMConfig):
             # The rest of kwargs is now passed to config
             llm_config = AutoConfig.for_model(model_name, **attrs)
         if type(llm_config) in cls._model_mapping.keys():
             llm = cls._model_mapping[type(llm_config)].from_pretrained(model_id, llm_config=llm_config, **attrs)
             if not return_runner_kwargs:
                 return llm
```

### Comparing `openllm-0.1.2/src/openllm/models/auto/modeling_auto.py` & `openllm-0.1.3/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.1.3/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.1.3/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/chatglm/__init__.py` & `openllm-0.1.3/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.1.3/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.1.3/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.1.3/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.1.3/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.1.3/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,20 @@
 
 
 class DollyV2(openllm.LLM["transformers.Pipeline", "transformers.PreTrainedTokenizer"]):
     __openllm_internal__ = True
 
     @property
     def import_kwargs(self):
-        return {
+        model_kwds = {
             "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
             "torch_dtype": torch.bfloat16,
-            "_tokenizer_padding_side": "left",
         }
+        tokenizer_kwds = {"padding_side": "left"}
+        return model_kwds, tokenizer_kwds
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     def import_model(
         self, model_id: str, tag: bentoml.Tag, *model_args: t.Any, tokenizer_kwds: dict[str, t.Any], **attrs: t.Any
     ) -> bentoml.Model:
```

### Comparing `openllm-0.1.2/src/openllm/models/falcon/__init__.py` & `openllm-0.1.3/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.1.3/src/openllm/models/falcon/configuration_falcon.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Refer to [Falcon's HuggingFace page](https://huggingface.co/tiiuae/falcon-7b) for more information.
     """
 
     __config__ = {
         "name_type": "lowercase",
         "trust_remote_code": True,
         "requires_gpu": True,
-        "timeout": 3600000,
+        "timeout": int(36e6),
         "url": "https://falconllm.tii.ae/",
         "requirements": ["einops", "xformers", "safetensors"],
         "default_id": "tiiuae/falcon-7b",
         "model_ids": [
             "tiiuae/falcon-7b",
             "tiiuae/falcon-40b",
             "tiiuae/falcon-7b-instruct",
```

### Comparing `openllm-0.1.2/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.1.3/src/openllm/models/falcon/modeling_falcon.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,20 @@
 
 
 class Falcon(openllm.LLM["transformers.TextGenerationPipeline", "transformers.PreTrainedTokenizerFast"]):
     __openllm_internal__ = True
 
     @property
     def import_kwargs(self):
-        return {
+        model_kwds = {
             "torch_dtype": torch.bfloat16,
             "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
         }
+        tokenizer_kwds: dict[str, t.Any] = {}
+        return model_kwds, tokenizer_kwds
 
     def import_model(
         self, model_id: str, tag: bentoml.Tag, *model_args: t.Any, tokenizer_kwds: dict[str, t.Any], **attrs: t.Any
     ) -> bentoml.Model:
         trust_remote_code = attrs.pop("trust_remote_code", True)
         torch_dtype = attrs.pop("torch_dtype", torch.bfloat16)
         device_map = attrs.pop("device_map", "auto")
@@ -68,19 +70,26 @@
             # NOTE: We need to free the cache after saving here so that we can load it back later on.
             gc.collect()
             torch.cuda.empty_cache()
 
     def load_model(self, tag: bentoml.Tag, *args: t.Any, **attrs: t.Any) -> t.Any:
         torch_dtype = attrs.pop("torch_dtype", torch.bfloat16)
         device_map = attrs.pop("device_map", "auto")
+        trust_remote_code = attrs.pop("trust_remote_code", True)
 
         _ref = bentoml.transformers.get(tag)
-
-        model = bentoml.transformers.load_model(_ref, device_map=device_map, torch_dtype=torch_dtype, **attrs)
-        return transformers.pipeline("text-generation", model=model, tokenizer=_ref.custom_objects["tokenizer"])
+        return transformers.pipeline(
+            "text-generation",
+            model=_ref.path,
+            tokenizer=_ref.custom_objects["tokenizer"],
+            trust_remote_code=trust_remote_code,
+            device_map=device_map,
+            torch_dtype=torch_dtype,
+            **attrs,
+        )
 
     def sanitize_parameters(
         self,
         prompt: str,
         max_new_tokens: int | None = None,
         top_k: int | None = None,
         num_return_sequences: int | None = None,
```

### Comparing `openllm-0.1.2/src/openllm/models/flan_t5/__init__.py` & `openllm-0.1.3/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.1.3/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.1.3/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.1.3/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.1.3/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.1.3/src/openllm/models/gptj/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/gptj/__init__.py` & `openllm-0.1.3/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/llama/__init__.py` & `openllm-0.1.3/src/openllm/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/roberta/__init__.py` & `openllm-0.1.3/src/openllm_client/runtimes/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-raise NotImplementedError("This module is not implemented yet.")
+from .grpc import GrpcClient as GrpcClient
+from .http import HTTPClient as HTTPClient
```

### Comparing `openllm-0.1.2/src/openllm/models/stablelm/__init__.py` & `openllm-0.1.3/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.1.3/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.1.3/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,21 @@
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.load_in_mha = True if not torch.cuda.is_available() else False
 
     @property
     def import_kwargs(self):
-        return {
+        model_kwds = {
             "torch_dtype": torch.float16 if torch.cuda.is_available() else torch.float32,
             "load_in_8bit": False,
             "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
         }
+        tokenizer_kwds: dict[str, t.Any] = {}
+        return model_kwds, tokenizer_kwds
 
     def sanitize_parameters(
         self,
         prompt: str,
         temperature: float | None = None,
         max_new_tokens: int | None = None,
         top_k: int | None = None,
```

### Comparing `openllm-0.1.2/src/openllm/models/starcoder/__init__.py` & `openllm-0.1.3/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.1.3/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.1.3/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,20 +41,21 @@
     __openllm_internal__ = True
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     @property
     def import_kwargs(self):
-        return {
-            "_tokenizer_padding_side": "left",
+        model_kwds = {
             "device_map": "auto" if torch.cuda.is_available() and torch.cuda.device_count() > 1 else None,
             "load_in_8bit": True if torch.cuda.device_count() > 1 else False,
             "torch_dtype": torch.float16,
         }
+        tokenizer_kwds = {"padding_side": "left"}
+        return model_kwds, tokenizer_kwds
 
     def import_model(
         self,
         model_id: str,
         tag: bentoml.Tag,
         *model_args: t.Any,
         tokenizer_kwds: dict[str, t.Any],
```

### Comparing `openllm-0.1.2/src/openllm/utils/__init__.py` & `openllm-0.1.3/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/analytics.py` & `openllm-0.1.3/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/dantic.py` & `openllm-0.1.3/src/openllm/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.1.3/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.1.3/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.1.3/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.1.3/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.1.3/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/import_utils.py` & `openllm-0.1.3/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm/utils/lazy.py` & `openllm-0.1.3/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm_client/__init__.py` & `openllm-0.1.3/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm_client/_prompt.py` & `openllm-0.1.3/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm_client/cache/__init__.py` & `openllm-0.1.3/src/openllm_client/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm_client/cache/inmemory.py` & `openllm-0.1.3/src/openllm_client/cache/inmemory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm_client/runtimes/__init__.py` & `openllm-0.1.3/src/openllm/__about__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,10 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from .grpc import GrpcClient as GrpcClient
-from .http import HTTPClient as HTTPClient
+__version__ = "0.1.3"
```

### Comparing `openllm-0.1.2/src/openllm_client/runtimes/base.py` & `openllm-0.1.3/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm_client/runtimes/grpc.py` & `openllm-0.1.3/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/src/openllm_client/runtimes/http.py` & `openllm-0.1.3/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tests/__init__.py` & `openllm-0.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tests/test_configuration.py` & `openllm-0.1.3/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tests/_strategies/__init__.py` & `openllm-0.1.3/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tests/_strategies/_configuration.py` & `openllm-0.1.3/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tests/models/flan_t5/__init__.py` & `openllm-0.1.3/tests/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tests/models/flan_t5/test_modeling_flan_t5.py` & `openllm-0.1.3/tests/models/flan_t5/test_modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tools/assert-model-table-latest` & `openllm-0.1.3/tools/assert-model-table-latest`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tools/run-release-action` & `openllm-0.1.3/tools/run-release-action`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tools/update-optional-dependencies.py` & `openllm-0.1.3/tools/update-optional-dependencies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/tools/update-readme.py` & `openllm-0.1.3/tools/update-readme.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     with open(os.path.join(ROOT, "pyproject.toml"), "r") as f:
         deps = tomlkit.parse(f.read()).value["project"]["optional-dependencies"]
 
     with open(os.path.join(ROOT, "README.md"), "r") as f:
         readme = f.readlines()
 
     start_index, stop_index = readme.index(START_COMMENT), readme.index(END_COMMENT)
-    formatted: dict[t.Literal["Model", "CPU", "GPU", "URL", "Installation", "Model Ids"], list[str]] = {
+    formatted: dict[t.Literal["Model", "CPU", "GPU", "URL", "Installation", "Model Ids"], list[str | list[str]]] = {
         "Model": [],
         "URL": [],
         "CPU": [],
         "GPU": [],
         "Installation": [],
         "Model Ids": [],
     }
@@ -66,26 +66,29 @@
 
     # NOTE: headers
     meta += ["<tr>\n"]
     meta.extend([f"<th>{header}</th>\n" for header in formatted.keys() if header not in ("URL",)])
     meta += ["</tr>\n"]
     # NOTE: rows
     for name, url, cpu, gpu, installation, model_ids in t.cast(
-        t.Iterable[t.Tuple[str, str, str, str, str, str]], zip(*formatted.values())
+        t.Iterable[t.Tuple[str, str, str, str, str, t.List[str]]], zip(*formatted.values())
     ):
         meta += "<tr>\n"
         meta.extend(
             [
                 f"\n<td><a href={url}>{name}</a></td>\n",
                 f"<td>{cpu}</td>\n",
                 f"<td>{gpu}</td>\n",
                 f"<td>\n\n{installation}\n\n</td>\n",
             ]
         )
-        meta.append("<td>\n\n" + "\n".join(["<li><code>" + lid + "</code></li>" for lid in model_ids]) + "\n\n</td>\n")
+        format_with_links: list[str] = []
+        for lid in model_ids:
+            format_with_links.append(f"<li><a href=https://huggingface.co/{lid}><code>{lid}</code></a></li>")
+        meta.append("<td>\n\n<ul>" + "\n".join(format_with_links) + "</ul>\n\n</td>\n")
         meta += "</tr>\n"
     meta.extend(["</table>\n", "\n"])
 
     readme = readme[:start_index] + [START_COMMENT] + meta + [END_COMMENT] + readme[stop_index + 1 :]
 
     with open(os.path.join(ROOT, "README.md"), "w") as f:
         f.writelines(readme)
```

### Comparing `openllm-0.1.2/typings/attr/__init__.pyi` & `openllm-0.1.3/typings/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/attr/exceptions.pyi` & `openllm-0.1.3/typings/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/attr/validators.pyi` & `openllm-0.1.3/typings/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/click_option_group/__init__.pyi` & `openllm-0.1.3/typings/click_option_group/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/click_option_group/_core.pyi` & `openllm-0.1.3/typings/click_option_group/_core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/click_option_group/_decorators.pyi` & `openllm-0.1.3/typings/click_option_group/_decorators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/click_option_group/_helpers.pyi` & `openllm-0.1.3/typings/click_option_group/_helpers.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/deepmerge/merger.pyi` & `openllm-0.1.3/typings/deepmerge/merger.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/deepmerge/strategy/core.pyi` & `openllm-0.1.3/typings/deepmerge/strategy/core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/typings/deepmerge/strategy/set.pyi` & `openllm-0.1.3/typings/deepmerge/strategy/set.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/.gitignore` & `openllm-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/LICENSE.md` & `openllm-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/README.md` & `openllm-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -138,19 +138,19 @@
 ```bash
 pip install "openllm[flan-t5]"
 ```
 
 </td>
 <td>
 
-<li><code>google/flan-t5-small</code></li>
-<li><code>google/flan-t5-base</code></li>
-<li><code>google/flan-t5-large</code></li>
-<li><code>google/flan-t5-xl</code></li>
-<li><code>google/flan-t5-xxl</code></li>
+<ul><li><a href=https://huggingface.co/google/flan-t5-small><code>google/flan-t5-small</code></a></li>
+<li><a href=https://huggingface.co/google/flan-t5-base><code>google/flan-t5-base</code></a></li>
+<li><a href=https://huggingface.co/google/flan-t5-large><code>google/flan-t5-large</code></a></li>
+<li><a href=https://huggingface.co/google/flan-t5-xl><code>google/flan-t5-xl</code></a></li>
+<li><a href=https://huggingface.co/google/flan-t5-xxl><code>google/flan-t5-xxl</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/databrickslabs/dolly>dolly-v2</a></td>
 <td>✅</td>
@@ -160,17 +160,17 @@
 ```bash
 pip install openllm
 ```
 
 </td>
 <td>
 
-<li><code>databricks/dolly-v2-3b</code></li>
-<li><code>databricks/dolly-v2-7b</code></li>
-<li><code>databricks/dolly-v2-12b</code></li>
+<ul><li><a href=https://huggingface.co/databricks/dolly-v2-3b><code>databricks/dolly-v2-3b</code></a></li>
+<li><a href=https://huggingface.co/databricks/dolly-v2-7b><code>databricks/dolly-v2-7b</code></a></li>
+<li><a href=https://huggingface.co/databricks/dolly-v2-12b><code>databricks/dolly-v2-12b</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/THUDM/ChatGLM-6B>chatglm</a></td>
 <td>❌</td>
@@ -180,17 +180,17 @@
 ```bash
 pip install "openllm[chatglm]"
 ```
 
 </td>
 <td>
 
-<li><code>thudm/chatglm-6b</code></li>
-<li><code>thudm/chatglm-6b-int8</code></li>
-<li><code>thudm/chatglm-6b-int4</code></li>
+<ul><li><a href=https://huggingface.co/thudm/chatglm-6b><code>thudm/chatglm-6b</code></a></li>
+<li><a href=https://huggingface.co/thudm/chatglm-6b-int8><code>thudm/chatglm-6b-int8</code></a></li>
+<li><a href=https://huggingface.co/thudm/chatglm-6b-int4><code>thudm/chatglm-6b-int4</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/bigcode-project/starcoder>starcoder</a></td>
 <td>❌</td>
@@ -200,16 +200,16 @@
 ```bash
 pip install "openllm[starcoder]"
 ```
 
 </td>
 <td>
 
-<li><code>bigcode/starcoder</code></li>
-<li><code>bigcode/starcoderbase</code></li>
+<ul><li><a href=https://huggingface.co/bigcode/starcoder><code>bigcode/starcoder</code></a></li>
+<li><a href=https://huggingface.co/bigcode/starcoderbase><code>bigcode/starcoderbase</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://falconllm.tii.ae/>falcon</a></td>
 <td>❌</td>
@@ -219,18 +219,18 @@
 ```bash
 pip install "openllm[falcon]"
 ```
 
 </td>
 <td>
 
-<li><code>tiiuae/falcon-7b</code></li>
-<li><code>tiiuae/falcon-40b</code></li>
-<li><code>tiiuae/falcon-7b-instruct</code></li>
-<li><code>tiiuae/falcon-40b-instruct</code></li>
+<ul><li><a href=https://huggingface.co/tiiuae/falcon-7b><code>tiiuae/falcon-7b</code></a></li>
+<li><a href=https://huggingface.co/tiiuae/falcon-40b><code>tiiuae/falcon-40b</code></a></li>
+<li><a href=https://huggingface.co/tiiuae/falcon-7b-instruct><code>tiiuae/falcon-7b-instruct</code></a></li>
+<li><a href=https://huggingface.co/tiiuae/falcon-40b-instruct><code>tiiuae/falcon-40b-instruct</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/Stability-AI/StableLM>stablelm</a></td>
 <td>✅</td>
@@ -240,18 +240,18 @@
 ```bash
 pip install openllm
 ```
 
 </td>
 <td>
 
-<li><code>stabilityai/stablelm-tuned-alpha-3b</code></li>
-<li><code>stabilityai/stablelm-tuned-alpha-7b</code></li>
-<li><code>stabilityai/stablelm-base-alpha-3b</code></li>
-<li><code>stabilityai/stablelm-base-alpha-7b</code></li>
+<ul><li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-3b><code>stabilityai/stablelm-tuned-alpha-3b</code></a></li>
+<li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b><code>stabilityai/stablelm-tuned-alpha-7b</code></a></li>
+<li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-3b><code>stabilityai/stablelm-base-alpha-3b</code></a></li>
+<li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-7b><code>stabilityai/stablelm-base-alpha-7b</code></a></li></ul>
 
 </td>
 </tr>
 </table>
 
 <!-- update-readme.py: stop -->
```

#### html2text {}

```diff
@@ -52,40 +52,41 @@
 specification. Users can also specify different variants of the model to be
 served, by providing the `--model-id` argument, e.g.: ```bash openllm start
 flan-t5 --model-id google/flan-t5-large ``` Use the `openllm models` command to
 see the list of models and their variants supported in OpenLLM. ## ð§©
 Supported Models The following models are currently supported in OpenLLM. By
 default, OpenLLM doesn't include dependencies to run all models. The extra
 model-specific dependencies can be installed with the instructions below:
- Model     CPU GPU Installation                    Model Ids
-                                                   google/flan-t5-small
-                   ```bash pip install "openllm    google/flan-t5-base
- flan-t5   ââ[flan-t5]" ```                  google/flan-t5-large
-                                                   google/flan-t5-xl
-                                                   google/flan-t5-xxl
-                                                   databricks/dolly-v2-3b
- dolly-v2  ââ```bash pip install openllm ``` databricks/dolly-v2-7b
-                                                   databricks/dolly-v2-12b
-                   ```bash pip install "openllm    thudm/chatglm-6b
- chatglm   ââ[chatglm]" ```                  thudm/chatglm-6b-int8
-                                                   thudm/chatglm-6b-int4
- starcoder ââ```bash pip install "openllm    bigcode/starcoder
-                   [starcoder]" ```                bigcode/starcoderbase
-                                                   tiiuae/falcon-7b
- falcon    ââ```bash pip install "openllm    tiiuae/falcon-40b
-                   [falcon]" ```                   tiiuae/falcon-7b-instruct
-                                                   tiiuae/falcon-40b-instruct
-                                                   stabilityai/stablelm-tuned-
-                                                   alpha-3b
-                                                   stabilityai/stablelm-tuned-
- stablelm  ââ```bash pip install openllm ``` alpha-7b
-                                                   stabilityai/stablelm-base-
-                                                   alpha-3b
-                                                   stabilityai/stablelm-base-
-                                                   alpha-7b
+Model     CPU GPU Installation                 Model Ids
+                                                   * google/flan-t5-small
+                  ```bash pip install "openllm     * google/flan-t5-base
+flan-t5   ââ[flan-t5]" ```                   * google/flan-t5-large
+                                                   * google/flan-t5-xl
+                                                   * google/flan-t5-xxl
+                  ```bash pip install openllm      * databricks/dolly-v2-3b
+dolly-v2  ââ```                              * databricks/dolly-v2-7b
+                                                   * databricks/dolly-v2-12b
+                  ```bash pip install "openllm     * thudm/chatglm-6b
+chatglm   ââ[chatglm]" ```                   * thudm/chatglm-6b-int8
+                                                   * thudm/chatglm-6b-int4
+starcoder ââ```bash pip install "openllm     * bigcode/starcoder
+                  [starcoder]" ```                 * bigcode/starcoderbase
+                                                   * tiiuae/falcon-7b
+                  ```bash pip install "openllm     * tiiuae/falcon-40b
+falcon    ââ[falcon]" ```                    * tiiuae/falcon-7b-instruct
+                                                   * tiiuae/falcon-40b-
+                                                     instruct
+                                                   * stabilityai/stablelm-
+                                                     tuned-alpha-3b
+                                                   * stabilityai/stablelm-
+stablelm  ââ```bash pip install openllm        tuned-alpha-7b
+                  ```                              * stabilityai/stablelm-
+                                                     base-alpha-3b
+                                                   * stabilityai/stablelm-
+                                                     base-alpha-7b
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
```

### Comparing `openllm-0.1.2/pyproject.toml` & `openllm-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.2/PKG-INFO` & `openllm-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm
 Author-email: Aaron Pham <aarnphm@bentoml.com>, BentoML Team <contact@bentoml.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
@@ -202,19 +202,19 @@
 ```bash
 pip install "openllm[flan-t5]"
 ```
 
 </td>
 <td>
 
-<li><code>google/flan-t5-small</code></li>
-<li><code>google/flan-t5-base</code></li>
-<li><code>google/flan-t5-large</code></li>
-<li><code>google/flan-t5-xl</code></li>
-<li><code>google/flan-t5-xxl</code></li>
+<ul><li><a href=https://huggingface.co/google/flan-t5-small><code>google/flan-t5-small</code></a></li>
+<li><a href=https://huggingface.co/google/flan-t5-base><code>google/flan-t5-base</code></a></li>
+<li><a href=https://huggingface.co/google/flan-t5-large><code>google/flan-t5-large</code></a></li>
+<li><a href=https://huggingface.co/google/flan-t5-xl><code>google/flan-t5-xl</code></a></li>
+<li><a href=https://huggingface.co/google/flan-t5-xxl><code>google/flan-t5-xxl</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/databrickslabs/dolly>dolly-v2</a></td>
 <td>✅</td>
@@ -224,17 +224,17 @@
 ```bash
 pip install openllm
 ```
 
 </td>
 <td>
 
-<li><code>databricks/dolly-v2-3b</code></li>
-<li><code>databricks/dolly-v2-7b</code></li>
-<li><code>databricks/dolly-v2-12b</code></li>
+<ul><li><a href=https://huggingface.co/databricks/dolly-v2-3b><code>databricks/dolly-v2-3b</code></a></li>
+<li><a href=https://huggingface.co/databricks/dolly-v2-7b><code>databricks/dolly-v2-7b</code></a></li>
+<li><a href=https://huggingface.co/databricks/dolly-v2-12b><code>databricks/dolly-v2-12b</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/THUDM/ChatGLM-6B>chatglm</a></td>
 <td>❌</td>
@@ -244,17 +244,17 @@
 ```bash
 pip install "openllm[chatglm]"
 ```
 
 </td>
 <td>
 
-<li><code>thudm/chatglm-6b</code></li>
-<li><code>thudm/chatglm-6b-int8</code></li>
-<li><code>thudm/chatglm-6b-int4</code></li>
+<ul><li><a href=https://huggingface.co/thudm/chatglm-6b><code>thudm/chatglm-6b</code></a></li>
+<li><a href=https://huggingface.co/thudm/chatglm-6b-int8><code>thudm/chatglm-6b-int8</code></a></li>
+<li><a href=https://huggingface.co/thudm/chatglm-6b-int4><code>thudm/chatglm-6b-int4</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/bigcode-project/starcoder>starcoder</a></td>
 <td>❌</td>
@@ -264,16 +264,16 @@
 ```bash
 pip install "openllm[starcoder]"
 ```
 
 </td>
 <td>
 
-<li><code>bigcode/starcoder</code></li>
-<li><code>bigcode/starcoderbase</code></li>
+<ul><li><a href=https://huggingface.co/bigcode/starcoder><code>bigcode/starcoder</code></a></li>
+<li><a href=https://huggingface.co/bigcode/starcoderbase><code>bigcode/starcoderbase</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://falconllm.tii.ae/>falcon</a></td>
 <td>❌</td>
@@ -283,18 +283,18 @@
 ```bash
 pip install "openllm[falcon]"
 ```
 
 </td>
 <td>
 
-<li><code>tiiuae/falcon-7b</code></li>
-<li><code>tiiuae/falcon-40b</code></li>
-<li><code>tiiuae/falcon-7b-instruct</code></li>
-<li><code>tiiuae/falcon-40b-instruct</code></li>
+<ul><li><a href=https://huggingface.co/tiiuae/falcon-7b><code>tiiuae/falcon-7b</code></a></li>
+<li><a href=https://huggingface.co/tiiuae/falcon-40b><code>tiiuae/falcon-40b</code></a></li>
+<li><a href=https://huggingface.co/tiiuae/falcon-7b-instruct><code>tiiuae/falcon-7b-instruct</code></a></li>
+<li><a href=https://huggingface.co/tiiuae/falcon-40b-instruct><code>tiiuae/falcon-40b-instruct</code></a></li></ul>
 
 </td>
 </tr>
 <tr>
 
 <td><a href=https://github.com/Stability-AI/StableLM>stablelm</a></td>
 <td>✅</td>
@@ -304,18 +304,18 @@
 ```bash
 pip install openllm
 ```
 
 </td>
 <td>
 
-<li><code>stabilityai/stablelm-tuned-alpha-3b</code></li>
-<li><code>stabilityai/stablelm-tuned-alpha-7b</code></li>
-<li><code>stabilityai/stablelm-base-alpha-3b</code></li>
-<li><code>stabilityai/stablelm-base-alpha-7b</code></li>
+<ul><li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-3b><code>stabilityai/stablelm-tuned-alpha-3b</code></a></li>
+<li><a href=https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b><code>stabilityai/stablelm-tuned-alpha-7b</code></a></li>
+<li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-3b><code>stabilityai/stablelm-base-alpha-3b</code></a></li>
+<li><a href=https://huggingface.co/stabilityai/stablelm-base-alpha-7b><code>stabilityai/stablelm-base-alpha-7b</code></a></li></ul>
 
 </td>
 </tr>
 </table>
 
 <!-- update-readme.py: stop -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm Version: 0.1.2 Summary: OpenLLM: REST/gRPC
+Metadata-Version: 2.1 Name: openllm Version: 0.1.3 Summary: OpenLLM: REST/gRPC
 API server for running any open Large-Language Model - StableLM, Llama, Alpaca,
 Dolly, Flan-T5, Custom Project-URL: Documentation, https://github.com/bentoml/
 openllm#readme Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm Author-email: Aaron
 Pham
 bentoml.com>, BentoML Team
 bentoml.com> License-Expression: Apache-2.0 License-File: LICENSE.md Keywords:
@@ -91,40 +91,41 @@
 specification. Users can also specify different variants of the model to be
 served, by providing the `--model-id` argument, e.g.: ```bash openllm start
 flan-t5 --model-id google/flan-t5-large ``` Use the `openllm models` command to
 see the list of models and their variants supported in OpenLLM. ## ð§©
 Supported Models The following models are currently supported in OpenLLM. By
 default, OpenLLM doesn't include dependencies to run all models. The extra
 model-specific dependencies can be installed with the instructions below:
- Model     CPU GPU Installation                    Model Ids
-                                                   google/flan-t5-small
-                   ```bash pip install "openllm    google/flan-t5-base
- flan-t5   ââ[flan-t5]" ```                  google/flan-t5-large
-                                                   google/flan-t5-xl
-                                                   google/flan-t5-xxl
-                                                   databricks/dolly-v2-3b
- dolly-v2  ââ```bash pip install openllm ``` databricks/dolly-v2-7b
-                                                   databricks/dolly-v2-12b
-                   ```bash pip install "openllm    thudm/chatglm-6b
- chatglm   ââ[chatglm]" ```                  thudm/chatglm-6b-int8
-                                                   thudm/chatglm-6b-int4
- starcoder ââ```bash pip install "openllm    bigcode/starcoder
-                   [starcoder]" ```                bigcode/starcoderbase
-                                                   tiiuae/falcon-7b
- falcon    ââ```bash pip install "openllm    tiiuae/falcon-40b
-                   [falcon]" ```                   tiiuae/falcon-7b-instruct
-                                                   tiiuae/falcon-40b-instruct
-                                                   stabilityai/stablelm-tuned-
-                                                   alpha-3b
-                                                   stabilityai/stablelm-tuned-
- stablelm  ââ```bash pip install openllm ``` alpha-7b
-                                                   stabilityai/stablelm-base-
-                                                   alpha-3b
-                                                   stabilityai/stablelm-base-
-                                                   alpha-7b
+Model     CPU GPU Installation                 Model Ids
+                                                   * google/flan-t5-small
+                  ```bash pip install "openllm     * google/flan-t5-base
+flan-t5   ââ[flan-t5]" ```                   * google/flan-t5-large
+                                                   * google/flan-t5-xl
+                                                   * google/flan-t5-xxl
+                  ```bash pip install openllm      * databricks/dolly-v2-3b
+dolly-v2  ââ```                              * databricks/dolly-v2-7b
+                                                   * databricks/dolly-v2-12b
+                  ```bash pip install "openllm     * thudm/chatglm-6b
+chatglm   ââ[chatglm]" ```                   * thudm/chatglm-6b-int8
+                                                   * thudm/chatglm-6b-int4
+starcoder ââ```bash pip install "openllm     * bigcode/starcoder
+                  [starcoder]" ```                 * bigcode/starcoderbase
+                                                   * tiiuae/falcon-7b
+                  ```bash pip install "openllm     * tiiuae/falcon-40b
+falcon    ââ[falcon]" ```                    * tiiuae/falcon-7b-instruct
+                                                   * tiiuae/falcon-40b-
+                                                     instruct
+                                                   * stabilityai/stablelm-
+                                                     tuned-alpha-3b
+                                                   * stabilityai/stablelm-
+stablelm  ââ```bash pip install openllm        tuned-alpha-7b
+                  ```                              * stabilityai/stablelm-
+                                                     base-alpha-3b
+                                                   * stabilityai/stablelm-
+                                                     base-alpha-7b
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
```

