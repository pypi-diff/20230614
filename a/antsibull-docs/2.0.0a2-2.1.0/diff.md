# Comparing `tmp/antsibull_docs-2.0.0a2.tar.gz` & `tmp/antsibull_docs-2.1.0.tar.gz`

## Comparing `antsibull_docs-2.0.0a2.tar` & `antsibull_docs-2.1.0.tar`

### file list

```diff
@@ -1,499 +1,514 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.flake8
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.git-blame-ignore-revs
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.pylintrc.automated
--rw-r--r--   0        0        0    21944 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/CHANGELOG.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/LICENSE
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/antsibull-docs.cfg
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/codecov.yml
--rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/noxfile.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.github/dependabot.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.github/patchback.yml
--rw-r--r--   0        0        0     8888 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.github/workflows/antsibull-docs.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.github/workflows/build-css.yml
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.github/workflows/nox.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.reuse/dep5
--rw-r--r--   0        0        0    26550 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/changelogs/changelog.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/changelogs/fragments/.keep
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/docs/schemas.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/app_context.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/augment_docs.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/collection_config.py
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/collection_links.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/constants.py
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/env_variables.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/extra_docs.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/lint_extra_docs.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/lint_helpers.py
--rw-r--r--   0        0        0    23794 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/lint_plugin_docs.py
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/process_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/py.typed
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/rstcheck.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/__init__.py
--rw-r--r--   0        0        0    25734 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/antsibull_docs.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/__init__.py
--rw-r--r--   0        0        0    10952 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/_build.py
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/collection.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/current.py
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/devel.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/lint_collection_docs.py
--rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/plugin.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/sphinx_init.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/stable.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/__init__.py
--rw-r--r--   0        0        0   127036 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/ansible_2_10_routing.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/__init__.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_callback_plugins.rst.j2
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_collections.rst.j2
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_collections_by_namespace.rst.j2
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_env_variables.rst.j2
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_plugins.rst.j2
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin-deprecation.rst.j2
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin-error.rst.j2
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin-redirect.rst.j2
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin-tombstone.rst.j2
--rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin.rst.j2
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugins_by_collection.rst.j2
--rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/role.rst.j2
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/attributes.rst.j2
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/choiceslist.rst.j2
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/deprecates.rst.j2
--rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/parameters.rst.j2
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/returnvalues.rst.j2
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/version_added.rst.j2
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/_gitignore.j2
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/build_sh.j2
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/conf_py.j2
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/requirements_txt.j2
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/__init__.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/ansible_doc.py
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/fqcn.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/parsing.py
--rw-r--r--   0        0        0    17280 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/routing.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/jinja2/__init__.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/jinja2/environment.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/jinja2/filters.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/jinja2/tests.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/markup/__init__.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/markup/_counter.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/markup/htmlify.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/markup/rstify.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/markup/semantic_helper.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/ansible_doc.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/app_context.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/collection_config.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/collection_links.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/__init__.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/ansible_doc.py
--rw-r--r--   0        0        0    25409 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/base.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/callback.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/module.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/plugin.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/positional.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/role.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/utils/__init__.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/utils/collection_name_transformer.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/utils/get_pkg_data.py
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/vendored/ansible.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/__init__.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/collections.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/hierarchy.py
--rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/indexes.py
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/plugin_stubs.py
--rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/plugins.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/__init__.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/antsibull-minimal.css
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/antsibull-minimal.css.license
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/assets.py
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/roles.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/css/antsibull-minimal.scss
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/css/browserslistrc
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/css/build.sh
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/css/cssnano.config.js
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/argcomplete.pyi
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/rstcheck.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/__init__.pyi
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/constants.pyi
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/release.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/cli/__init__.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/cli/arguments.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/collections/list.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/galaxy/collection.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/module_utils/_text.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/module_utils/common/json.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/plugins/loader.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/utils/collection_loader.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/ansible/utils/plugin_docs.pyi
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/jinja2/utils.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/rstcheck_core/__init__.pyi
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/rstcheck_core/checker.pyi
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/rstcheck_core/config.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/stubs/rstcheck_core/types.pyi
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/validate-html.py
--rw-r--r--   0        0        0    49283 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-all.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-all.json.license
--rw-r--r--   0        0        0    17296 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns.col1.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns.col1.json.license
--rw-r--r--   0        0        0    23778 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns.col2.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns.col2.json.license
--rw-r--r--   0        0        0    39823 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns2.col.json.license
--rw-r--r--   0        0        0    20278 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns2.flatcol.json.license
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-all.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-all.json.license
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-ns.col1.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-ns.col1.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-ns.col2.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-ns.col2.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-ns2.col.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-galaxy-cache-ns2.flatcol.json.license
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-version.output
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible-version.output.license
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/ansible_doc_caching.py
--rwxr-xr-x   0        0        0     2482 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/build-docs-baseline.sh
--rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/build-sphinx-init-baseline.sh
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/sanitize-ansible-doc-dump.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/sanitize-ansible-galaxy-list.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/test.rst
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/test_docs_baseline.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/test_docs_linting.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/test_sphinx_init_baseline.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/environment_variables.rst
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_become.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_cache.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_callback.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_cliconf.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_connection.rst
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_filter.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_inventory.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_lookup.rst
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_module.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_role.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_shell.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_strategy.rst
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_test.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_vars.rst
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/index.rst
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/index.rst
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_become.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_cache.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_callback.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_cliconf.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_connection.rst
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_filter.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_inventory.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_lookup.rst
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_role.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_shell.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_strategy.rst
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_test.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_vars.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/index.rst
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/index.rst
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/environment_variables.rst
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     6889 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/build.sh
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/conf.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/requirements.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/.gitignore
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      809 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/build.sh
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/conf.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/requirements.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/build.sh
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/conf.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/requirements.txt
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/rst/index.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/.gitignore
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/build.sh
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/conf.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/rst/index.rst
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/bar_filter.rst
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/bar_test.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/environment_variables.rst
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo2_module.rst
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_become.rst
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_cache.rst
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_connection.rst
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_filter.rst
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_inventory.rst
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_lookup.rst
--rw-r--r--   0        0        0    12315 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_module.rst
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_role.rst
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_strategy.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_test.rst
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_vars.rst
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/is_bar_test.rst
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index.rst
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_become.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_cache.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_callback.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_cliconf.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_connection.rst
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_filter.rst
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_inventory.rst
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_lookup.rst
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_module.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_role.rst
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_shell.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_strategy.rst
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_test.rst
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/index_vars.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/index.rst
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col1/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col1/galaxy.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col1/plugins/module_utils/empty.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/galaxy.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/config.yml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/extra-docs.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/rst/filter_guide.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/meta/runtime.yml
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/extra-docs.yml
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/meta/runtime.yml
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/main.yml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/roles/foo/tasks/main.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/flatcol/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/flatcol/galaxy.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/flatcol/docs/docsite/config.yml
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/test_schema.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_become.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_become.json.license
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_become_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_become_results.json.license
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cache.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cache.json.license
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cache_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cache_results.json.license
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_callback.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_callback.json.license
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_callback_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_callback_results.json.license
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cliconf.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cliconf.json.license
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cliconf_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cliconf_results.json.license
--rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_connection.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_connection.json.license
--rw-r--r--   0        0        0    23697 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_connection_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_connection_results.json.license
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_filter.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_filter.json.license
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_filter_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_filter_results.json.license
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_httpapi.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_httpapi.json.license
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_httpapi_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_httpapi_results.json.license
--rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_inventory.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_inventory.json.license
--rw-r--r--   0        0        0    33185 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_inventory_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_inventory_results.json.license
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_lookup.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_lookup.json.license
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_lookup_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_lookup_results.json.license
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_module.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_module.json.license
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_module_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_module_results.json.license
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_netconf.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_netconf.json.license
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_netconf_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_netconf_results.json.license
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_role.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_role.json.license
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_role_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_role_results.json.license
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_shell.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_shell.json.license
--rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_shell_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_shell_results.json.license
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_strategy.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_strategy.json.license
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_strategy_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_strategy_results.json.license
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_test.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_test.json.license
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_test_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_test_results.json.license
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_vars.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_vars.json.license
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_vars_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_vars_results.json.license
--rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/ssh_connection.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/ssh_connection.json.license
--rw-r--r--   0        0        0    56342 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/ssh_connection_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/functional/schema/good_data/ssh_connection_results.json.license
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/units/test_jinja2.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/units/markup/test_counter.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/tests/units/markup/test_markup.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/.gitignore
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/README.md
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 antsibull_docs-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.flake8
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.pylintrc.automated
+-rw-r--r--   0        0        0    24826 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/antsibull-docs.cfg
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/codecov.yml
+-rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/noxfile.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.github/patchback.yml
+-rw-r--r--   0        0        0     8888 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.github/workflows/antsibull-docs.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.github/workflows/build-css.yml
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.reuse/dep5
+-rw-r--r--   0        0        0    30212 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/changelogs/fragments/.keep
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/docs/schemas.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/__init__.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/app_context.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/augment_docs.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/collection_config.py
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/collection_links.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/constants.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/env_variables.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/extra_docs.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/lint_extra_docs.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/lint_helpers.py
+-rw-r--r--   0        0        0    26187 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/lint_plugin_docs.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/plugin_docs.py
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/process_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/py.typed
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/rstcheck.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/__init__.py
+-rw-r--r--   0        0        0    26939 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/antsibull_docs.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/__init__.py
+-rw-r--r--   0        0        0    11552 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/_build.py
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/collection.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/current.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/devel.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/lint_collection_docs.py
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/plugin.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/stable.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/__init__.py
+-rw-r--r--   0        0        0   127036 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/ansible_2_10_routing.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/__init__.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_callback_plugins.rst.j2
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_collections.rst.j2
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_collections_by_namespace.rst.j2
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_env_variables.rst.j2
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_plugins.rst.j2
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin-deprecation.rst.j2
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin-error.rst.j2
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin-redirect.rst.j2
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin-tombstone.rst.j2
+-rw-r--r--   0        0        0    17353 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin.rst.j2
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugins_by_collection.rst.j2
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/role.rst.j2
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/attributes.rst.j2
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/choiceslist.rst.j2
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/deprecates.rst.j2
+-rw-r--r--   0        0        0    14559 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/parameters.rst.j2
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/returnvalues.rst.j2
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/version_added.rst.j2
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/_gitignore.j2
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/build_sh.j2
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/conf_py.j2
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/requirements_txt.j2
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/__init__.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/ansible_doc.py
+-rw-r--r--   0        0        0     7304 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/fqcn.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/parsing.py
+-rw-r--r--   0        0        0    17280 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/routing.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/jinja2/__init__.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/jinja2/environment.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/jinja2/filters.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/jinja2/tests.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/markup/__init__.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/markup/_counter.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/markup/htmlify.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/markup/rstify.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/markup/semantic_helper.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/ansible_doc.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/app_context.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/collection_config.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/collection_links.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/__init__.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/ansible_doc.py
+-rw-r--r--   0        0        0    25409 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/base.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/callback.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/module.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/plugin.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/positional.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/role.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/utils/collection_name_transformer.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/utils/get_pkg_data.py
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/vendored/ansible.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/write_docs/__init__.py
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/write_docs/collections.py
+-rw-r--r--   0        0        0     8031 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/write_docs/hierarchy.py
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/write_docs/indexes.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/write_docs/plugin_stubs.py
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/antsibull_docs/write_docs/plugins.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/__init__.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/antsibull-minimal.css
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/antsibull-minimal.css.license
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/assets.py
+-rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/roles.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/css/browserslistrc
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/css/build.sh
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/src/sphinx_antsibull_ext/css/cssnano.config.js
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/argcomplete.pyi
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/rstcheck.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/__init__.pyi
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/constants.pyi
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/release.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/cli/__init__.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/cli/arguments.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/collections/list.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/galaxy/collection.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/module_utils/_text.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/module_utils/common/json.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/plugins/loader.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/utils/collection_loader.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/ansible/utils/plugin_docs.pyi
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/jinja2/utils.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/rstcheck_core/__init__.pyi
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/rstcheck_core/checker.pyi
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/rstcheck_core/config.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/stubs/rstcheck_core/types.pyi
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/validate-html.py
+-rw-r--r--   0        0        0  1040575 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-all-others.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-all-others.json.license
+-rw-r--r--   0        0        0  1038729 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-all.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-all.json.license
+-rw-r--r--   0        0        0    17296 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns.col1.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns.col1.json.license
+-rw-r--r--   0        0        0    26488 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns.col2.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns.col2.json.license
+-rw-r--r--   0        0        0    40797 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns2.col.json.license
+-rw-r--r--   0        0        0    20537 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns2.flatcol.json.license
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-all-others.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-all-others.json.license
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-all.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-all.json.license
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-ns.col1.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-ns.col1.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-ns.col2.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-ns.col2.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-ns2.col.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-galaxy-cache-ns2.flatcol.json.license
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-version.output
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible-version.output.license
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/ansible_doc_caching.py
+-rwxr-xr-x   0        0        0     3141 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/build-docs-baseline.sh
+-rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/build-sphinx-init-baseline.sh
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/sanitize-ansible-doc-dump.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/sanitize-ansible-galaxy-list.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/test.rst
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/test_docs_baseline.py
+-rw-r--r--   0        0        0    83036 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/test_docs_linting.py
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/test_sphinx_init_baseline.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/environment_variables.rst
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_become.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_cache.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_callback.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_connection.rst
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_filter.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_inventory.rst
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_lookup.rst
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_module.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_role.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_shell.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_strategy.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_test.rst
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_vars.rst
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/index.rst
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12427 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_become.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_cache.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_callback.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_connection.rst
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_filter.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_inventory.rst
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_lookup.rst
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_role.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_shell.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_strategy.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_test.rst
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_vars.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/index.rst
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12427 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12427 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/build.sh
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/requirements.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/.gitignore
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      809 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/build.sh
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/conf.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/requirements.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/build.sh
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/requirements.txt
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/rst/index.rst
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/.gitignore
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/build.sh
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/conf.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/rst/index.rst
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/bar_test.rst
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_become.rst
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst
+-rw-r--r--   0        0        0    12427 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_module.rst
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_role.rst
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_test.rst
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/index.rst
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/is_bar_test.rst
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index.rst
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_become.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_cache.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_callback.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_connection.rst
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_filter.rst
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_inventory.rst
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_lookup.rst
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_module.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_role.rst
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_shell.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_strategy.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_test.rst
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/index_vars.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/index.rst
+-rw-r--r--   0        0        0     9572 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col1/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col1/galaxy.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col1/plugins/module_utils/empty.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/galaxy.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/config.yml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/extra-docs.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/rst/filter_guide.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/meta/runtime.yml
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/config.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/extra-docs.yml
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/meta/runtime.yml
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/is_bar.yml -> bar.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/main.yml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/tasks/main.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/flatcol/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/flatcol/galaxy.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/flatcol/docs/docsite/config.yml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/other-collections/ansible_collections/ext/col/galaxy.yml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/test_schema.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_become.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_become.json.license
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_become_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_become_results.json.license
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cache.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cache.json.license
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cache_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cache_results.json.license
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_callback.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_callback.json.license
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_callback_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_callback_results.json.license
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cliconf.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cliconf.json.license
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cliconf_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cliconf_results.json.license
+-rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_connection.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_connection.json.license
+-rw-r--r--   0        0        0    23697 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_connection_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_connection_results.json.license
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_filter.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_filter.json.license
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_filter_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_filter_results.json.license
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_httpapi.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_httpapi.json.license
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_httpapi_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_httpapi_results.json.license
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_inventory.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_inventory.json.license
+-rw-r--r--   0        0        0    33185 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_inventory_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_inventory_results.json.license
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_lookup.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_lookup.json.license
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_lookup_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_lookup_results.json.license
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_module.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_module.json.license
+-rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_module_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_module_results.json.license
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_netconf.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_netconf.json.license
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_netconf_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_netconf_results.json.license
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_role.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_role.json.license
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_role_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_role_results.json.license
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_shell.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_shell.json.license
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_shell_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_shell_results.json.license
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_strategy.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_strategy.json.license
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_strategy_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_strategy_results.json.license
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_test.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_test.json.license
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_test_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_test_results.json.license
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_vars.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_vars.json.license
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_vars_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/one_vars_results.json.license
+-rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/ssh_connection.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/ssh_connection.json.license
+-rw-r--r--   0        0        0    56342 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/ssh_connection_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/functional/schema/good_data/ssh_connection_results.json.license
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/units/test_jinja2.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/units/markup/test_counter.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/tests/units/markup/test_markup.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/.gitignore
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/README.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 antsibull_docs-2.1.0/PKG-INFO
```

### Comparing `antsibull_docs-2.0.0a2/.pylintrc.automated` & `antsibull_docs-2.1.0/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/CHANGELOG.rst` & `antsibull_docs-2.1.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 ===================================================================
 antsibull-docs -- Ansible Documentation Build Scripts Release Notes
 ===================================================================
 
 .. contents:: Topics
 
 
-v2.0.0a2
-========
+v2.1.0
+======
 
 Release Summary
 ---------------
 
-Hotfix to make ``sphinx-init`` work properly.
+Feature and bugfix release with many improvements related to semantic markup and validation.
+
+Minor Changes
+-------------
+
+- Add option ``--disallow-unknown-collection-refs`` to disallow references to other collections than the one covered by ``--validate-collection-refs`` (https://github.com/ansible-community/antsibull-docs/pull/157).
+- Add option ``--validate-collection-refs`` to the ``lint-collection-docs`` subcommand to also control which references to plugin/module/role names in (other) collections and their options and return values should be validated (https://github.com/ansible-community/antsibull-docs/pull/157).
+- Add the new collection config field ``envvar_directives`` which allows to declare which environment variables are declared with an ``.. envvar::`` directive in the collection's extra docsite documentation. This is used, next to the plugin configuration information and the ansible-core configuration information, to determine whether an environment variable is referencable or not (https://github.com/ansible-community/antsibull-docs/pull/166).
+- Add the roles ``:ansenvvar:`` and ``:ansenvvarref:`` to the antsibull-docs Sphinx extension (https://github.com/ansible-community/antsibull-docs/pull/166).
+- Render ``E(...)`` markup with ``:ansenvvarref:`` or ``:ansenvvar:`` depending on whether the environment variable is known to be referencable or not (https://github.com/ansible-community/antsibull-docs/pull/166).
+- When linting markup in collection docs, validate plugin/module/role names, and also option/return value names for other plugins/modules/roles in the same collection, (transitively) dependent collections, and ansible.builtin (https://github.com/ansible-community/antsibull-docs/pull/157).
+- When linting semantic markup in collection docs, also accept aliases when checking ``O()`` values (https://github.com/ansible-community/antsibull-docs/pull/155).
+- When refering to markup in multi-paragraph texts, like ``description``, now includes the paragraph number in error messages (https://github.com/ansible-community/antsibull-docs/pull/163).
 
 Bugfixes
 --------
 
-- Bump version range of antsibull-docs requirement written by ``sphinx-init`` subcommand to ``>= 2.0.0a2, < 3.0.0``. Previously, this was set to ``>=2.0.0, <3.0.0`` which could not be satisfied (https://github.com/ansible-community/antsibull-docs/pull/149).
+- Allow role entrypoint deprecations without having to specify the collection the role is removed from (https://github.com/ansible-community/antsibull-docs/pull/156).
+- Indent module/plugin and role entrypoint deprecations correctly if 'Why' or 'Alternative' texts need more than one line (https://github.com/ansible-community/antsibull-docs/pull/156).
+- When collecting collection dependencies for the ``lint-collection-docs`` subcommand, a bug prevented the duplicate detection to work (https://github.com/ansible-community/antsibull-docs/pull/160).
 
-v2.0.0a1
-========
+v2.0.0
+======
 
 Release Summary
 ---------------
 
-Pre-release of new major 2.0.0 release.
+Major new release that drops support for older Python and Ansible/ansible-base/ansible-core versions.
 
 Major Changes
 -------------
 
 - Change pyproject build backend from ``poetry-core`` to ``hatchling``. ``pip install antsibull-docs`` works exactly the same as before, but some users may be affected depending on how they build/install the project (https://github.com/ansible-community/antsibull-docs/pull/115).
 
 Minor Changes
 -------------
 
 - Allow to use the currently installed ansible-core version for the ``devel`` and ``stable`` subcommands (https://github.com/ansible-community/antsibull-docs/pull/121).
 - Ansibull-docs now no longer depends directly on ``sh`` (https://github.com/ansible-community/antsibull-docs/pull/122).
+- Bump version range of antsibull-docs requirement written by ``sphinx-init`` subcommand to ``>= 2.0.0, < 3.0.0``. Previously, this was set to ``>=2.0.0a2, <3.0.0`` (https://github.com/ansible-community/antsibull-docs/pull/151).
 - Now depends antsibull-core 2.0.0 or newer; antsibull-core 1.x.y is no longer supported (https://github.com/ansible-community/antsibull-docs/pull/122).
 - Remove residual compatability code for Python 3.6 and 3.7 (https://github.com/ansible-community/antsibull-docs/pulls/70).
 - Support a per-collection docs config file ``docs/docsite/config.yml``. It is also linted by the ``lint-collection-docs`` subcommand (https://github.com/ansible-community/antsibull-docs/pull/134).
 - The antsibull-docs requirement in the ``requirements.txt`` file created by the sphinx-init subcommand now has version range ``>= 2.0.0, < 3.0.0`` (https://github.com/ansible-community/antsibull-docs/pull/126).
 - The dependency `antsibull-docs-parser <https://github.com/ansible-community/antsibull-docs-parser>`__ has been added and is used for processing Ansible markup (https://github.com/ansible-community/antsibull-docs/pull/124).
 
 Breaking Changes / Porting Guide
@@ -50,14 +65,15 @@
 - No longer removes ``PYTHONPATH`` from the environment when calling ``ansible``, ``ansible-galaxy``, or ``ansible-doc`` outside a self-created venv (https://github.com/ansible-community/antsibull-docs/pull/121).
 - No longer supports Ansible 2.9, ansible-base 2.10, and ansible-core 2.11 and 2.12. The minimum required ansible-core version is 2.13. This allows for simpler and more efficient docs parsing and information retrieval (https://github.com/ansible-community/antsibull-docs/pull/120).
 - The ``ansible-doc`` and ``ansible-internal`` values for ``doc_parsing_backend`` in the configuration file have been removed. Change the value to ``auto`` for best compatibility (https://github.com/ansible-community/antsibull-docs/pull/120).
 
 Bugfixes
 --------
 
+- Bump version range of antsibull-docs requirement written by ``sphinx-init`` subcommand to ``>= 2.0.0a2, < 3.0.0``. Previously, this was set to ``>=2.0.0, <3.0.0`` which could not be satisfied (https://github.com/ansible-community/antsibull-docs/pull/149).
 - Use ``doc_parsing_backend`` from the application context instead of the library context. This prevents removal of ``doc_parsing_backend`` from the antsibull-core library context (https://github.com/ansible-community/antsibull-docs/pull/125).
 
 v1.11.0
 =======
 
 Release Summary
 ---------------
```

### Comparing `antsibull_docs-2.0.0a2/LICENSE` & `antsibull_docs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/antsibull-docs.cfg` & `antsibull_docs-2.1.0/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/noxfile.py` & `antsibull_docs-2.1.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/.github/workflows/antsibull-docs.yml` & `antsibull_docs-2.1.0/.github/workflows/antsibull-docs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/.github/workflows/build-css.yml` & `antsibull_docs-2.1.0/.github/workflows/build-css.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/.github/workflows/nox.yml` & `antsibull_docs-2.1.0/.github/workflows/nox.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/changelogs/changelog.yaml` & `antsibull_docs-2.1.0/changelogs/changelog.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -405,14 +405,26 @@
         https://github.com/ansible-community/antsibull-docs/pull/90).
       release_summary: Feature release.
     fragments:
     - 1.9.0.yml
     - 90-callbacks.yml
     - 92-sphinx-init-build-sh.yml
     release_date: '2023-01-12'
+  2.0.0:
+    changes:
+      minor_changes:
+      - Bump version range of antsibull-docs requirement written by ``sphinx-init``
+        subcommand to ``>= 2.0.0, < 3.0.0``. Previously, this was set to ``>=2.0.0a2,
+        <3.0.0`` (https://github.com/ansible-community/antsibull-docs/pull/151).
+      release_summary: Major new release that drops support for older Python and Ansible/ansible-base/ansible-core
+        versions.
+    fragments:
+    - 151-changes.yml
+    - 2.0.0.yml
+    release_date: '2023-05-19'
   2.0.0a1:
     changes:
       breaking_changes:
       - 'Disable flatmapping for all collections except community.general < 6.0.0
         and community.network < 5.0.0. You can enable flatmapping for your collection
         by setting ``flatmap: true`` in ``docs/docsite/config.yml`` (https://github.com/ansible-community/antsibull-docs/pull/134).'
       - Drop support for Python 3.6, 3.7, and 3.8 (https://github.com/ansible-community/antsibull-docs/pull/115)."
@@ -464,7 +476,51 @@
       - Bump version range of antsibull-docs requirement written by ``sphinx-init``
         subcommand to ``>= 2.0.0a2, < 3.0.0``. Previously, this was set to ``>=2.0.0,
         <3.0.0`` which could not be satisfied (https://github.com/ansible-community/antsibull-docs/pull/149).
       release_summary: Hotfix to make ``sphinx-init`` work properly.
     fragments:
     - 2.0.0a2.yml
     release_date: '2023-05-10'
+  2.1.0:
+    changes:
+      bugfixes:
+      - Allow role entrypoint deprecations without having to specify the collection
+        the role is removed from (https://github.com/ansible-community/antsibull-docs/pull/156).
+      - Indent module/plugin and role entrypoint deprecations correctly if 'Why' or
+        'Alternative' texts need more than one line (https://github.com/ansible-community/antsibull-docs/pull/156).
+      - When collecting collection dependencies for the ``lint-collection-docs`` subcommand,
+        a bug prevented the duplicate detection to work (https://github.com/ansible-community/antsibull-docs/pull/160).
+      minor_changes:
+      - Add option ``--disallow-unknown-collection-refs`` to disallow references to
+        other collections than the one covered by ``--validate-collection-refs`` (https://github.com/ansible-community/antsibull-docs/pull/157).
+      - Add option ``--validate-collection-refs`` to the ``lint-collection-docs``
+        subcommand to also control which references to plugin/module/role names in
+        (other) collections and their options and return values should be validated
+        (https://github.com/ansible-community/antsibull-docs/pull/157).
+      - Add the new collection config field ``envvar_directives`` which allows to
+        declare which environment variables are declared with an ``.. envvar::`` directive
+        in the collection's extra docsite documentation. This is used, next to the
+        plugin configuration information and the ansible-core configuration information,
+        to determine whether an environment variable is referencable or not (https://github.com/ansible-community/antsibull-docs/pull/166).
+      - Add the roles ``:ansenvvar:`` and ``:ansenvvarref:`` to the antsibull-docs
+        Sphinx extension (https://github.com/ansible-community/antsibull-docs/pull/166).
+      - Render ``E(...)`` markup with ``:ansenvvarref:`` or ``:ansenvvar:`` depending
+        on whether the environment variable is known to be referencable or not (https://github.com/ansible-community/antsibull-docs/pull/166).
+      - When linting markup in collection docs, validate plugin/module/role names,
+        and also option/return value names for other plugins/modules/roles in the
+        same collection, (transitively) dependent collections, and ansible.builtin
+        (https://github.com/ansible-community/antsibull-docs/pull/157).
+      - When linting semantic markup in collection docs, also accept aliases when
+        checking ``O()`` values (https://github.com/ansible-community/antsibull-docs/pull/155).
+      - When refering to markup in multi-paragraph texts, like ``description``, now
+        includes the paragraph number in error messages (https://github.com/ansible-community/antsibull-docs/pull/163).
+      release_summary: Feature and bugfix release with many improvements related to
+        semantic markup and validation.
+    fragments:
+    - 155-aliases.yml
+    - 156-indent-deprecation.yml
+    - 157-other-collections.yml
+    - 160-dependency-collection.yml
+    - 163-lint-paragraph.yml
+    - 166-envvars.yml
+    - 2.1.0.yml
+    release_date: '2023-06-14'
```

### Comparing `antsibull_docs-2.0.0a2/changelogs/config.yaml` & `antsibull_docs-2.1.0/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/docs/schemas.rst` & `antsibull_docs-2.1.0/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/app_context.py` & `antsibull_docs-2.1.0/src/antsibull_docs/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/augment_docs.py` & `antsibull_docs-2.1.0/src/antsibull_docs/augment_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/collection_config.py` & `antsibull_docs-2.1.0/src/antsibull_docs/collection_config.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/collection_links.py` & `antsibull_docs-2.1.0/src/antsibull_docs/collection_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/constants.py` & `antsibull_docs-2.1.0/src/antsibull_docs/constants.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/env_variables.py` & `antsibull_docs-2.1.0/src/antsibull_docs/env_variables.py`

 * *Files 12% similar despite different names*

```diff
@@ -110,27 +110,52 @@
                     break
             variable_info.description = value
 
 
 def collect_referenced_environment_variables(
     plugin_info: Mapping[str, Mapping[str, t.Any]],
     ansible_config: Mapping[str, Mapping[str, t.Any]],
-) -> Mapping[str, EnvironmentVariableInfo]:
+) -> tuple[Mapping[str, EnvironmentVariableInfo], set[str]]:
     """
     Collect referenced environment variables that are not defined in the ansible-core
     configuration.
 
     :arg plugin_info: Mapping of plugin type to a mapping of plugin name to plugin record.
     :arg ansible_config: The Ansible base configuration (``lib/ansible/config/base.yml``).
-    :returns: A Mapping of environment variable name to an environment variable infomation object.
+    :returns: A tuple consisting of a
+        Mapping of environment variable name to an environment variable infomation object,
+        and a set of environment variable names that are part of the ansible-core
+        configuration.
     """
     core_envs = {"ANSIBLE_CONFIG"}
     for config in ansible_config.values():
         if config.get("env"):
             for env in config["env"]:
                 core_envs.add(env["name"])
 
     other_variables, other_variable_description = _collect_env_vars_and_descriptions(
         plugin_info, core_envs
     )
     _augment_env_var_descriptions(other_variables, other_variable_description)
-    return other_variables
+    return other_variables, core_envs
+
+
+def collect_referable_envvars(
+    referenced_env_vars: Mapping[str, EnvironmentVariableInfo],
+    core_env_vars: set[str],
+    collection_metadata: Mapping[str, AnsibleCollectionMetadata],
+) -> set[str]:
+    """
+    :arg referenced_env_vars: A Mapping of environment variable name to an
+        environment variable infomation object.
+    :arg core_env_vars: Set of environment variable names that are part of the
+        ansible-core configuration.
+    :arg collection_metadata: A Mapping of collection names to collection metadata
+        objects.
+    :returns: A set of environment variables that can be referenced via the
+        ``:envvar:`` role.
+    """
+    referable_envvars = set(referenced_env_vars)
+    referable_envvars.update(core_env_vars)
+    for collection_meta in collection_metadata.values():
+        referable_envvars.update(collection_meta.docs_config.envvar_directives)
+    return referable_envvars
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/extra_docs.py` & `antsibull_docs-2.1.0/src/antsibull_docs/extra_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/lint_extra_docs.py` & `antsibull_docs-2.1.0/src/antsibull_docs/lint_extra_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/lint_helpers.py` & `antsibull_docs-2.1.0/src/antsibull_docs/lint_helpers.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/process_docs.py` & `antsibull_docs-2.1.0/src/antsibull_docs/process_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/rstcheck.py` & `antsibull_docs-2.1.0/src/antsibull_docs/rstcheck.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/antsibull_docs.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/antsibull_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         raise InvalidArgumentError(
             f"{args.dest_dir} must only be writable by the owner"
         )
 
     try:
         if writable_via_acls(args.dest_dir, euid):
             raise InvalidArgumentError(
-                f"Filesystem acls grant write on {args.dest_dir} to" " additional users"
+                f"Filesystem acls grant write on {args.dest_dir} to additional users"
             )
     except UnableToCheck:
         # We've done our best but some systems don't even have acls on their filesystem so we can't
         # error here.
         pass
 
 
@@ -309,28 +309,28 @@
         help="Do not create the collection index and plugin indexes."
         " This option is deprecated in favor of --no-indexes",
     )
 
     parser = get_toplevel_parser(
         prog=program_name,
         package="antsibull_docs",
-        description="Script to manage generated documentation for" " ansible",
+        description="Script to manage generated documentation for ansible",
     )
     subparsers = parser.add_subparsers(
         title="Subcommands", dest="command", help="for help use: `SUBCOMMANDS -h`"
     )
     subparsers.required = True
 
     #
     # Document the next version of ansible
     #
     devel_parser = subparsers.add_parser(
         "devel",
         parents=[docs_parser, cache_parser, whole_site_parser, template_parser],
-        description="Generate documentation for the next major" " release of Ansible",
+        description="Generate documentation for the next major release of Ansible",
     )
     devel_parser.add_argument(
         "--pieces-file",
         default=DEFAULT_PIECES_FILE,
         help="File containing a list of collections to include",
     )
     devel_parser.add_argument(
@@ -344,15 +344,15 @@
 
     #
     # Document a released version of ansible
     #
     stable_parser = subparsers.add_parser(
         "stable",
         parents=[docs_parser, cache_parser, whole_site_parser, template_parser],
-        description="Generate documentation for a current" " version of ansible",
+        description="Generate documentation for a current version of ansible",
     )
     stable_parser.add_argument(
         "--deps-file",
         required=True,
         help="File which contains the list of collections and"
         " versions which were included in this version of Ansible",
     )
@@ -384,15 +384,15 @@
 
     #
     # Document one or more specified collections
     #
     collection_parser = subparsers.add_parser(
         "collection",
         parents=[docs_parser, whole_site_parser, template_parser],
-        description="Generate documentation for specified" " collections",
+        description="Generate documentation for specified collections",
     )
     collection_parser.add_argument(
         "--collection-version",
         default="@latest",
         help="The version of the collection to document.  The special"
         ' version, "@latest" can be used to download and document the'
         " latest version from galaxy.",
@@ -447,15 +447,15 @@
 
     #
     # Create a Sphinx site template
     #
     sphinx_init_parser = subparsers.add_parser(
         "sphinx-init",
         parents=[docs_parser, template_parser, whole_site_parser],
-        description="Generate a Sphinx site template for a" " collection docsite",
+        description="Generate a Sphinx site template for a collection docsite",
     )
 
     sphinx_init_parser.add_argument(
         "--collection-version",
         default="@latest",
         help="The version of the collection to document.  The special"
         ' version, "@latest" can be used to download and document the'
@@ -554,32 +554,55 @@
     )
 
     #
     # Lint collection docs
     #
     lint_collection_docs_parser = subparsers.add_parser(
         "lint-collection-docs",
-        description="Collection extra docs linter" " for inclusion in docsite",
+        description="Collection extra docs linter for inclusion in docsite",
     )
 
     lint_collection_docs_parser.add_argument(
         "collection_root_path",
         metavar="/path/to/collection",
-        help="path to collection (directory that includes" " galaxy.yml)",
+        help="path to collection (directory that includes galaxy.yml)",
     )
     lint_collection_docs_parser.add_argument(
         "--plugin-docs",
         dest="plugin_docs",
         action=BooleanOptionalAction,
         default=False,
         help="Determine whether to also check RST file"
         " generation and schema and markup validation for"
         " plugins and roles in this collection.",
     )
     lint_collection_docs_parser.add_argument(
+        "--validate-collection-refs",
+        dest="validate_collections_refs",
+        choices=["self", "dependent", "all"],
+        default="dependent",
+        help="When --plugin-docs is specified, determine references to which"
+        " collections to validate.  'self' means only validate references to"
+        " this collection.  'dependent' means validating references to"
+        " collections this collection (transitively) depends on, including"
+        " references to ansible.builtin.  'all' means validating references"
+        " to all collections the linter can find.",
+    )
+    lint_collection_docs_parser.add_argument(
+        "--disallow-unknown-collection-refs",
+        dest="disallow_unknown_collection_refs",
+        action=BooleanOptionalAction,
+        default=False,
+        help="When --plugin-docs is specified, determine references to which"
+        " collections to validate.  'self' means only validate references to"
+        " this collection.  'dependent' means validating references to"
+        " collections this collection (transitively) depends on.  'all' means"
+        " validating references to all collections the linter can find.",
+    )
+    lint_collection_docs_parser.add_argument(
         "--skip-rstcheck",
         dest="skip_rstcheck",
         action=BooleanOptionalAction,
         default=False,
         help="When --plugin-docs is specified, do not run"
         " rstcheck on the generated RST files. This speeds"
         " up testing for large collections.",
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/_build.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/_build.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from ...docs_parsing.parsing import get_ansible_plugin_info
 from ...docs_parsing.routing import (
     find_stubs,
     load_all_collection_routing,
     remove_redirect_duplicates,
 )
 from ...env_variables import (
+    collect_referable_envvars,
     collect_referenced_environment_variables,
     load_ansible_config,
 )
 from ...extra_docs import load_collections_extra_docs
 from ...process_docs import (
     get_callback_plugin_contents,
     get_collection_contents,
@@ -156,17 +157,20 @@
                     print(
                         f"{plugin_name} {plugin_type}: {textwrap.indent(error, '    ').lstrip()}"
                     )
         return 1
 
     # Handle environment variables
     ansible_config = load_ansible_config(full_collection_metadata["ansible.builtin"])
-    referenced_env_vars = collect_referenced_environment_variables(
+    referenced_env_vars, core_env_vars = collect_referenced_environment_variables(
         new_plugin_info, ansible_config
     )
+    referable_envvars = collect_referable_envvars(
+        referenced_env_vars, core_env_vars, collection_metadata
+    )
 
     collection_namespaces = get_collection_namespaces(collection_to_plugin_info.keys())
 
     collection_url = CollectionNameTransformer(
         app_ctx.collection_url, "https://galaxy.ansible.com/{namespace}/{name}"
     )
     collection_install = CollectionNameTransformer(
@@ -181,46 +185,50 @@
                 collection_to_plugin_info,
                 collection_namespaces,
                 dest_dir,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 breadcrumbs=breadcrumbs,
                 for_official_docsite=for_official_docsite,
+                referable_envvars=referable_envvars,
             )
         )
         flog.notice("Finished writing collection index")
         asyncio.run(
             output_collection_namespace_indexes(
                 collection_namespaces,
                 dest_dir,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 breadcrumbs=breadcrumbs,
                 for_official_docsite=for_official_docsite,
+                referable_envvars=referable_envvars,
             )
         )
         flog.notice("Finished writing collection namespace index")
         asyncio.run(
             output_plugin_indexes(
                 plugin_contents,
                 collection_metadata,
                 dest_dir,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 for_official_docsite=for_official_docsite,
+                referable_envvars=referable_envvars,
             )
         )
         flog.notice("Finished writing plugin indexes")
         asyncio.run(
             output_callback_indexes(
                 callback_plugin_contents,
                 dest_dir,
                 collection_url=collection_url,
                 collection_install=collection_install,
                 for_official_docsite=for_official_docsite,
+                referable_envvars=referable_envvars,
             )
         )
         flog.notice("Finished writing callback plugin indexes")
 
     asyncio.run(
         output_indexes(
             collection_to_plugin_info,
@@ -229,28 +237,30 @@
             collection_install=collection_install,
             collection_metadata=collection_metadata,
             squash_hierarchy=squash_hierarchy,
             extra_docs_data=extra_docs_data,
             link_data=link_data,
             breadcrumbs=breadcrumbs,
             for_official_docsite=for_official_docsite,
+            referable_envvars=referable_envvars,
         )
     )
     flog.notice("Finished writing indexes")
 
     asyncio.run(
         output_all_plugin_stub_rst(
             stubs_info,
             dest_dir,
             collection_url=collection_url,
             collection_install=collection_install,
             collection_metadata=collection_metadata,
             link_data=link_data,
             squash_hierarchy=squash_hierarchy,
             for_official_docsite=for_official_docsite,
+            referable_envvars=referable_envvars,
         )
     )
     flog.debug("Finished writing plugin stubs")
 
     asyncio.run(
         output_all_plugin_rst(
             collection_to_plugin_info,
@@ -260,23 +270,27 @@
             collection_url=collection_url,
             collection_install=collection_install,
             collection_metadata=collection_metadata,
             link_data=link_data,
             squash_hierarchy=squash_hierarchy,
             use_html_blobs=use_html_blobs,
             for_official_docsite=for_official_docsite,
+            referable_envvars=referable_envvars,
         )
     )
     flog.debug("Finished writing plugin docs")
 
     asyncio.run(
         output_extra_docs(dest_dir, extra_docs_data, squash_hierarchy=squash_hierarchy)
     )
     flog.debug("Finished writing extra docs")
 
     asyncio.run(
         output_environment_variables(
-            dest_dir, referenced_env_vars, squash_hierarchy=squash_hierarchy
+            dest_dir,
+            referenced_env_vars,
+            squash_hierarchy=squash_hierarchy,
+            referable_envvars=referable_envvars,
         )
     )
     flog.debug("Finished writing environment variables")
     return 0
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/collection.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/collection.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/current.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/current.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/devel.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/devel.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/lint_collection_docs.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/lint_collection_docs.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     flog = mlog.fields(func="lint_collection_docs")
     flog.notice("Begin collection docs linting")
 
     app_ctx = app_context.app_ctx.get()
 
     collection_root = app_ctx.extra["collection_root_path"]
     plugin_docs = app_ctx.extra["plugin_docs"]
+    validate_collections_refs = app_ctx.extra["validate_collections_refs"]
+    disallow_unknown_collection_refs = app_ctx.extra["disallow_unknown_collection_refs"]
     skip_rstcheck = app_ctx.extra["skip_rstcheck"]
     disallow_semantic_markup = app_ctx.extra["disallow_semantic_markup"]
 
     flog.notice("Linting docs config file")
     errors = lint_collection_config(collection_root)
 
     flog.notice("Linting extra docs files")
@@ -58,14 +60,16 @@
             "ansible-galaxy collection install {namespace}.{name}",
         )
         errors.extend(
             lint_collection_plugin_docs(
                 collection_root,
                 collection_url=collection_url,
                 collection_install=collection_install,
+                validate_collections_refs=validate_collections_refs,
+                disallow_unknown_collection_refs=disallow_unknown_collection_refs,
                 skip_rstcheck=skip_rstcheck,
                 disallow_semantic_markup=disallow_semantic_markup,
             )
         )
 
     messages = sorted(
         (os.path.normpath(error[0]), error[1], error[2], error[3].lstrip())
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/plugin.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/plugin.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/sphinx_init.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/cli/doc_commands/stable.py` & `antsibull_docs-2.1.0/src/antsibull_docs/cli/doc_commands/stable.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/ansible_2_10_routing.yml` & `antsibull_docs-2.1.0/src/antsibull_docs/data/ansible_2_10_routing.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_callback_plugins.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_callback_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_collections.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_collections.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_collections_by_namespace.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_collections_by_namespace.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_env_variables.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_env_variables.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/list_of_plugins.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/list_of_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin-deprecation.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin-deprecation.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin-error.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin-error.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin-redirect.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin-redirect.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin-tombstone.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin-tombstone.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugin.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugin.rst.j2`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,16 @@
 :Removed in: version @{ doc['deprecated']['removed_in'] | rst_ify }@
 {% else %}
 :Removed in: a future release
 {% endif %}
 {% if doc['deprecated']['removed_from_collection'] and doc['deprecated']['removed_from_collection'] != collection %}
              of @{ doc['deprecated']['removed_from_collection'] | rst_ify }@
 {% endif %}
-:Why: @{ doc['deprecated']['why'] | rst_ify }@
-:Alternative: @{ doc['deprecated']['alternative'] | rst_ify }@
+:Why: @{ doc['deprecated']['why'] | rst_ify | indent(6) }@
+:Alternative: @{ doc['deprecated']['alternative'] | rst_ify | indent(14) }@
 {% endif %}
 
 {% if plugin_type == 'callback' %}
 Callback plugin
 ---------------
 
 {%   if doc['type'] == 'stdout' %}
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/plugins_by_collection.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/plugins_by_collection.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/role.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/role.rst.j2`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,16 @@
 {%     if ep_doc['deprecated']['removed_at_date'] %}
 :Removed in: major release after @{ ep_doc['deprecated']['removed_at_date'] | rst_ify(role_entrypoint=entry_point) }@
 {%     elif ep_doc['deprecated']['removed_in'] %}
 :Removed in: version @{ ep_doc['deprecated']['removed_in'] | rst_ify(role_entrypoint=entry_point) }@
 {%     else %}
 :Removed in: a future release
 {%     endif %}
-:Why: @{ ep_doc['deprecated']['why'] | rst_ify(role_entrypoint=entry_point) }@
-:Alternative: @{ ep_doc['deprecated']['alternative'] | rst_ify(role_entrypoint=entry_point) }@
+:Why: @{ ep_doc['deprecated']['why'] | rst_ify(role_entrypoint=entry_point) | indent(6) }@
+:Alternative: @{ ep_doc['deprecated']['alternative'] | rst_ify(role_entrypoint=entry_point) | indent(14) }@
 {%   endif %}
 
 Synopsis
 ^^^^^^^^
 
 .. Description
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/attributes.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/attributes.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/choiceslist.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/choiceslist.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/deprecates.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/deprecates.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/parameters.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/parameters.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/returnvalues.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/returnvalues.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/docsite/macros/version_added.rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/docsite/macros/version_added.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/build_sh.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/build_sh.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/conf_py.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/conf_py.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2` & `antsibull_docs-2.1.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/__init__.py` & `antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,38 +46,46 @@
     pass
 
 
 class ParsingError(Exception):
     """Error raised while parsing plugins for documentation."""
 
 
+def _get_existing_collections_path() -> str | None:
+    for env_var in ("ANSIBLE_COLLECTIONS_PATH", "ANSIBLE_COLLECTIONS_PATHS"):
+        if os.environ.get(env_var):
+            return os.environ[env_var]
+    return None
+
+
 def _get_environment(
     collection_dir: str | None,
     venv: VenvRunner | FakeVenvRunner,
+    keep_current_collections_path: bool = False,
 ) -> dict[str, str]:
     env = ANSIBLE_PATH_ENVIRON.copy()
     if isinstance(venv, VenvRunner):
         try:
             del env["PYTHONPATH"]
         except KeyError:
             # We just wanted to make sure there was no PYTHONPATH set...
             # all Python libs will come from the venv
             pass
+    for env_var in ("ANSIBLE_COLLECTIONS_PATH", "ANSIBLE_COLLECTIONS_PATHS"):
+        try:
+            del env[env_var]
+        except KeyError:
+            pass
+    existing_collections_path = _get_existing_collections_path()
     if collection_dir is not None:
+        if keep_current_collections_path and existing_collections_path:
+            collection_dir = f"{collection_dir}:{existing_collections_path}"
         env["ANSIBLE_COLLECTIONS_PATH"] = collection_dir
-    else:
-        # Copy ANSIBLE_COLLECTIONS_PATH and ANSIBLE_COLLECTIONS_PATHS from the
-        # original environment.
-        for env_var in ("ANSIBLE_COLLECTIONS_PATH", "ANSIBLE_COLLECTIONS_PATHS"):
-            try:
-                del env[env_var]
-            except KeyError:
-                pass
-            if env_var in os.environ:
-                env[env_var] = os.environ[env_var]
+    elif existing_collections_path:
+        env["ANSIBLE_COLLECTIONS_PATH"] = existing_collections_path
     return env
 
 
 class AnsibleCollectionMetadata:
     path: str
     version: str | None
     requires_ansible: str | None
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/ansible_doc.py` & `antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py` & `antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,40 +69,45 @@
     return meta.docs_config.flatmap
 
 
 async def get_ansible_plugin_info(
     venv: VenvRunner | FakeVenvRunner,
     collection_dir: str | None,
     collection_names: list[str] | None = None,
+    fetch_all_installed: bool = False,
 ) -> tuple[
     MutableMapping[str, MutableMapping[str, t.Any]],
     Mapping[str, AnsibleCollectionMetadata],
 ]:
     """
     Retrieve information about all of the Ansible Plugins. Requires ansible-core 2.13+.
 
     :arg venv: A VenvRunner into which Ansible has been installed.
     :arg collection_dir: Directory in which the collections have been installed.
                          If ``None``, the collections are assumed to be in the current
                          search path for Ansible.
     :arg collection_names: Optional list of collections. If specified, will only collect
                            information for plugins in these collections.
+    :arg fetch_all_installed: If set to ``True``, will also retrieve plugins of installed
+        collections outside ``collection_dir`` (if specified).
     :returns: An tuple. The first component is a nested directory structure that looks like:
 
             plugin_type:
                 plugin_name:  # Includes namespace and collection.
                     {information from ansible-doc --json.  See the ansible-doc documentation
                      for more info.}
 
         The second component is a Mapping of collection names to metadata.
     """
     flog = mlog.fields(func="get_ansible_plugin_info")
     flog.debug("Enter")
 
-    env = _get_environment(collection_dir, venv=venv)
+    env = _get_environment(
+        collection_dir, keep_current_collections_path=fetch_all_installed, venv=venv
+    )
 
     flog.debug("Retrieving and loading plugin documentation")
     if collection_names and len(collection_names) == 1:
         # ansible-doc only allows *one* filter
         ansible_doc_output = await _call_ansible_doc(venv, env, collection_names[0])
     else:
         ansible_doc_output = await _call_ansible_doc(venv, env)
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/fqcn.py` & `antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/fqcn.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/parsing.py` & `antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/parsing.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,27 +27,30 @@
 mlog = log.fields(mod=__name__)
 
 
 async def get_ansible_plugin_info(
     venv: VenvRunner | FakeVenvRunner,
     collection_dir: str | None,
     collection_names: list[str] | None = None,
+    fetch_all_installed: bool = False,
 ) -> tuple[
     MutableMapping[str, MutableMapping[str, t.Any]],
     Mapping[str, AnsibleCollectionMetadata],
 ]:
     """
     Retrieve information about all of the Ansible Plugins.
 
     :arg venv: A VenvRunner into which Ansible has been installed.
     :arg collection_dir: Directory in which the collections have been installed.
                          If ``None``, the collections are assumed to be in the current
                          search path for Ansible.
     :arg collection_names: Optional list of collections. If specified, will only collect
                            information for plugins in these collections.
+    :arg fetch_all_installed: If set to ``True``, will also retrieve plugins of installed
+        collections outside ``collection_dir`` (if specified).
     :returns: An tuple. The first component is a nested directory structure that looks like:
 
             plugin_type:
                 plugin_name:  # Includes namespace and collection.
                     {information from ansible-doc --json.  See the ansible-doc documentation
                      for more info.}
 
@@ -67,11 +70,14 @@
             raise RuntimeError(
                 f"Unsupported ansible-core version {version}. Need 2.13.0 or later."
             )
         doc_parsing_backend = "ansible-core-2.13"
         flog.debug(f"Auto-detected docs parsing backend: {doc_parsing_backend}")
     if doc_parsing_backend == "ansible-core-2.13":
         return await ansible_doc_core_213_get_ansible_plugin_info(
-            venv, collection_dir, collection_names=collection_names
+            venv,
+            collection_dir,
+            collection_names=collection_names,
+            fetch_all_installed=fetch_all_installed,
         )
 
     raise RuntimeError(f"Invalid value for doc_parsing_backend: {doc_parsing_backend}")
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/docs_parsing/routing.py` & `antsibull_docs-2.1.0/src/antsibull_docs/docs_parsing/routing.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/jinja2/environment.py` & `antsibull_docs-2.1.0/src/antsibull_docs/jinja2/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 def doc_environment(
     template_location: str | tuple[str, str],
     *,
     extra_filters: Mapping[str, t.Callable] | None = None,
     extra_tests: Mapping[str, t.Callable] | None = None,
     collection_url: CollectionNameTransformer | None = None,
     collection_install: CollectionNameTransformer | None = None,
+    referable_envvars: set[str] | None = None,
 ) -> Environment:
     loader: BaseLoader
     if isinstance(template_location, str) and os.path.exists(template_location):
         loader = FileSystemLoader(template_location)
     else:
         if isinstance(template_location, str):
             template_pkg = template_location
@@ -82,23 +83,24 @@
     )
     env.globals["xline"] = rst_xline
 
     # Can be removed (and template switched to use namespace) when we no longer need to build
     # with <Jinja-2.10
     env.globals["to_kludge_ns"] = to_kludge_ns
     env.globals["from_kludge_ns"] = from_kludge_ns
-    env.globals["reference_plugin_rst"] = reference_plugin_rst
     if "max" not in env.filters:
         # Jinja < 2.10
         env.filters["max"] = do_max
 
     if "tojson" not in env.filters:
         # Jinja < 2.9
         env.filters["tojson"] = json.dumps
 
+    env.globals["reference_plugin_rst"] = reference_plugin_rst
+    env.globals["referable_envvars"] = referable_envvars
     env.filters["rst_ify"] = rst_ify
     env.filters["html_ify"] = html_ify
     env.filters["fmt"] = rst_fmt
     env.filters["rst_code"] = rst_code
     env.filters["rst_escape"] = rst_escape
     env.filters["xline"] = rst_xline
     env.filters["documented_type"] = documented_type
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/jinja2/filters.py` & `antsibull_docs-2.1.0/src/antsibull_docs/jinja2/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
     )
 
     text, counts = rst_ify_impl(
         text,
         plugin_fqcn=plugin_fqcn,
         plugin_type=plugin_type,
         role_entrypoint=role_entrypoint,
+        referable_envvars=context.get("referable_envvars"),
     )
 
     flog.fields(counts=counts).info("Number of macros converted to rst equivalents")
     flog.debug("Leave")
     return text
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/jinja2/tests.py` & `antsibull_docs-2.1.0/src/antsibull_docs/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/markup/_counter.py` & `antsibull_docs-2.1.0/src/antsibull_docs/markup/_counter.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/markup/htmlify.py` & `antsibull_docs-2.1.0/src/antsibull_docs/markup/htmlify.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/markup/rstify.py` & `antsibull_docs-2.1.0/src/antsibull_docs/markup/rstify.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from __future__ import annotations
 
 import typing as t
 from collections.abc import Mapping
 
 from antsibull_docs_parser import dom
 from antsibull_docs_parser.parser import Context, parse
+from antsibull_docs_parser.rst import AntsibullRSTFormatter
 from antsibull_docs_parser.rst import rst_escape as _rst_escape
 from antsibull_docs_parser.rst import to_rst
 
 from ._counter import count as _count
 
 
 def rst_escape(value: t.Any, escape_ending_whitespace=False) -> str:
@@ -27,26 +28,42 @@
     return _rst_escape(value, escape_ending_whitespace=escape_ending_whitespace)
 
 
 def rst_code(value: str) -> str:
     """Write value as :code:`...` RST construct."""
     if not isinstance(value, str):
         value = str(value)
-    return f":code:`{rst_escape(value, escape_ending_whitespace=True)}`"
+    return f":code:`{_rst_escape(value, escape_ending_whitespace=True)}`"
+
+
+class CustomizedAntsibullRSTFormatter(AntsibullRSTFormatter):
+    def __init__(self, referable_envvars: set[str] | None = None):
+        self._referable_envvars = referable_envvars or set()
+
+    def format_env_variable(self, part: dom.EnvVariablePart) -> str:
+        envvar = part.name.split("=", 1)[0].strip()
+        if envvar in self._referable_envvars:
+            return f"\\ :ansenvvarref:`{_rst_escape(part.name, True)}`\\ "
+        return f"\\ :ansenvvar:`{_rst_escape(part.name, True)}`\\ "
 
 
 def rst_ify(
     text: str,
     *,
     plugin_fqcn: str | None = None,
     plugin_type: str | None = None,
     role_entrypoint: str | None = None,
+    referable_envvars: set[str] | None = None,
 ) -> tuple[str, Mapping[str, int]]:
     """convert symbols like I(this is in italics) to valid restructured text"""
     current_plugin: dom.PluginIdentifier | None = None
     if plugin_fqcn and plugin_type:
         current_plugin = dom.PluginIdentifier(fqcn=plugin_fqcn, type=plugin_type)
     context = Context(current_plugin=current_plugin, role_entrypoint=role_entrypoint)
     paragraphs = parse(text, context, errors="message")
-    text = to_rst(paragraphs, current_plugin=current_plugin)
+    text = to_rst(
+        paragraphs,
+        current_plugin=current_plugin,
+        formatter=CustomizedAntsibullRSTFormatter(referable_envvars),
+    )
     counts = _count(paragraphs)
     return text, counts
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/markup/semantic_helper.py` & `antsibull_docs-2.1.0/src/antsibull_docs/markup/semantic_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/ansible_doc.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/app_context.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/collection_config.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/collection_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,8 +9,14 @@
 # to initialize the attributes when data is loaded into them.
 # pyre-ignore-all-errors[13]
 
 import pydantic as p
 
 
 class CollectionConfig(p.BaseModel):
+    # Whether the collection uses flatmapping to flatten subdirectories in
+    # `plugins/*/`.
     flatmap: bool = False
+
+    # List of environment variables that are defined by `.. envvar::` directives
+    # in the extra docsite RST files.
+    envvar_directives: list[str] = []
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/collection_links.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/collection_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/__init__.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/ansible_doc.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/base.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/base.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/callback.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/callback.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/module.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/module.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/plugin.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/plugin.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/positional.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/positional.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/schemas/docs/role.py` & `antsibull_docs-2.1.0/src/antsibull_docs/schemas/docs/role.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """Schemas for the role documentation data."""
 
 # Ignore Unitialized attribute errors because BaseModel works some magic
 # to initialize the attributes when data is loaded into them.
 # pyre-ignore-all-errors[13]
 
 import typing as t
+from collections.abc import Mapping
 
 import pydantic as p
 
 from .base import (
     COLLECTION_NAME_F,
     AttributeSchema,
     AttributeSchemaActionGroup,
@@ -23,14 +24,16 @@
     DeprecationSchema,
     OptionsSchema,
     SeeAlsoLinkSchema,
     SeeAlsoModSchema,
     SeeAlsoRefSchema,
 )
 
+_SENTINEL = object()
+
 
 class InnerRoleOptionsSchema(OptionsSchema):
     options: dict[str, "InnerRoleOptionsSchema"] = {}
 
     @p.root_validator(pre=True)
     # pylint:disable=no-self-argument
     def allow_description_to_be_optional(cls, values):
@@ -69,7 +72,24 @@
 
 class RoleSchema(BaseModel):
     """Documentation for roles."""
 
     collection: str = COLLECTION_NAME_F
     entry_points: dict[str, RoleEntrypointSchema]
     path: str
+
+    @p.root_validator(pre=True)
+    # pylint:disable=no-self-argument
+    def add_entrypoint_deprecation_collection(cls, values):
+        entry_points = values.get("entry_points")
+        collection = values.get("collection")
+        if isinstance(entry_points, Mapping) and isinstance(collection, str):
+            for data in entry_points.values():
+                if isinstance(data, Mapping):
+                    deprecation = data.get("deprecated")
+                    if isinstance(deprecation, Mapping):
+                        removed_from_collection = deprecation.get(
+                            "removed_from_collection", _SENTINEL
+                        )
+                        if removed_from_collection is _SENTINEL:
+                            deprecation["removed_from_collection"] = collection
+        return values
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/utils/collection_name_transformer.py` & `antsibull_docs-2.1.0/src/antsibull_docs/utils/collection_name_transformer.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/utils/get_pkg_data.py` & `antsibull_docs-2.1.0/src/antsibull_docs/utils/get_pkg_data.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/vendored/ansible.py` & `antsibull_docs-2.1.0/src/antsibull_docs/vendored/ansible.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/__init__.py` & `antsibull_docs-2.1.0/src/antsibull_docs/write_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/collections.py` & `antsibull_docs-2.1.0/src/antsibull_docs/write_docs/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     extra_docs_data: Mapping[str, CollectionExtraDocsInfoT],
     link_data: Mapping[str, CollectionLinks],
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     squash_hierarchy: bool = False,
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
+    referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate collection-level index pages for the collections.
 
     :arg collection_to_plugin_info: Mapping of collection_name to Mapping of plugin_type to
         Mapping of plugin_name to short_description.
     :arg dest_dir: The directory to place the documentation in.
@@ -149,25 +150,27 @@
     :arg link_data: Dictionary mapping collection names to CollectionLinks.
     :kwarg squash_hierarchy: If set to ``True``, no directory hierarchy will be used.
         Undefined behavior if documentation for multiple collections are created.
     :kwarg breadcrumbs: Default True.  Set to False if breadcrumbs for collections should be
         disabled.  This will disable breadcrumbs but save on memory usage.
     :kwarg for_official_docsite: Default False.  Set to True to use wording specific for the
         official docsite on docs.ansible.com.
+    :kwarg referable_envvars: Optional set of environment variables that can be referenced.
     """
     flog = mlog.fields(func="output_indexes")
     flog.debug("Enter")
 
     if collection_metadata is None:
         collection_metadata = {}
 
     env = doc_environment(
         ("antsibull_docs.data", "docsite"),
         collection_url=collection_url,
         collection_install=collection_install,
+        referable_envvars=referable_envvars,
     )
     # Get the templates
     collection_plugins_tmpl = env.get_template("plugins_by_collection.rst.j2")
 
     writers = []
     lib_ctx = app_context.lib_ctx.get()
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/hierarchy.py` & `antsibull_docs-2.1.0/src/antsibull_docs/write_docs/hierarchy.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,34 +99,37 @@
     collection_to_plugin_info: CollectionInfoT,
     collection_namespaces: Mapping[str, list[str]],
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
+    referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate top-level collection index page for the collections.
 
     :arg collection_to_plugin_info: Mapping of collection_name to Mapping of plugin_type to
         Mapping of plugin_name to short_description.
     :arg collection_namespaces: Mapping from collection namespaces to list of collection names.
     :arg dest_dir: The directory to place the documentation in.
     :kwarg breadcrumbs: Default True.  Set to False if breadcrumbs for collections should be
         disabled.  This will disable breadcrumbs but save on memory usage.
     :kwarg for_official_docsite: Default False.  Set to True to use wording specific for the
         official docsite on docs.ansible.com.
+    :kwarg referable_envvars: Optional set of environment variables that can be referenced.
     """
     flog = mlog.fields(func="output_collection_index")
     flog.debug("Enter")
 
     env = doc_environment(
         ("antsibull_docs.data", "docsite"),
         collection_url=collection_url,
         collection_install=collection_install,
+        referable_envvars=referable_envvars,
     )
     # Get the templates
     collection_list_tmpl = env.get_template("list_of_collections.rst.j2")
 
     collection_toplevel = os.path.join(dest_dir, "collections")
     flog.fields(
         toplevel=collection_toplevel, exists=os.path.isdir(collection_toplevel)
@@ -150,32 +153,35 @@
 async def output_collection_namespace_indexes(
     collection_namespaces: Mapping[str, list[str]],
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     breadcrumbs: bool = True,
     for_official_docsite: bool = False,
+    referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate collection namespace index pages for the collections.
 
     :arg collection_namespaces: Mapping from collection namespaces to list of collection names.
     :arg dest_dir: The directory to place the documentation in.
     :kwarg breadcrumbs: Default True.  Set to False if breadcrumbs for collections should be
         disabled.  This will disable breadcrumbs but save on memory usage.
     :kwarg for_official_docsite: Default False.  Set to True to use wording specific for the
         official docsite on docs.ansible.com.
+    :kwarg referable_envvars: Optional set of environment variables that can be referenced.
     """
     flog = mlog.fields(func="output_collection_namespace_indexes")
     flog.debug("Enter")
 
     env = doc_environment(
         ("antsibull_docs.data", "docsite"),
         collection_url=collection_url,
         collection_install=collection_install,
+        referable_envvars=referable_envvars,
     )
     # Get the templates
     collection_list_tmpl = env.get_template("list_of_collections_by_namespace.rst.j2")
 
     writers = []
     lib_ctx = app_context.lib_ctx.get()
     async with asyncio_pool.AioPool(size=lib_ctx.thread_max) as pool:
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/indexes.py` & `antsibull_docs-2.1.0/src/antsibull_docs/write_docs/indexes.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,32 +90,35 @@
 
 async def output_callback_indexes(
     plugin_info: PluginCollectionInfoT,
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     for_official_docsite: bool = False,
+    referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate top-level callback plugin index pages for all callback plugins of a type in all
     collections.
 
     :arg plugin_info: Mapping of callback_type to Mapping of collection_name to Mapping of
         plugin_name to short_description.
     :arg dest_dir: The directory to place the documentation in.
     :kwarg for_official_docsite: Default False.  Set to True to use wording specific for the
         official docsite on docs.ansible.com.
+    :kwarg referable_envvars: Optional set of environment variables that can be referenced.
     """
     flog = mlog.fields(func="output_callback_indexes")
     flog.debug("Enter")
 
     env = doc_environment(
         ("antsibull_docs.data", "docsite"),
         collection_url=collection_url,
         collection_install=collection_install,
+        referable_envvars=referable_envvars,
     )
     # Get the templates
     plugin_list_tmpl = env.get_template("list_of_callback_plugins.rst.j2")
 
     collection_toplevel = os.path.join(dest_dir, "collections")
     flog.fields(
         toplevel=collection_toplevel, exists=os.path.isdir(collection_toplevel)
@@ -151,32 +154,35 @@
 async def output_plugin_indexes(
     plugin_info: PluginCollectionInfoT,
     collection_metadata: Mapping[str, AnsibleCollectionMetadata],
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     for_official_docsite: bool = False,
+    referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Generate top-level plugin index pages for all plugins of a type in all collections.
 
     :arg plugin_info: Mapping of plugin_type to Mapping of collection_name to Mapping of
         plugin_name to short_description.
     :arg collection_metadata: Dictionary mapping collection names to collection metadata objects.
     :arg dest_dir: The directory to place the documentation in.
     :kwarg for_official_docsite: Default False.  Set to True to use wording specific for the
         official docsite on docs.ansible.com.
+    :kwarg referable_envvars: Optional set of environment variables that can be referenced.
     """
     flog = mlog.fields(func="output_plugin_indexes")
     flog.debug("Enter")
 
     env = doc_environment(
         ("antsibull_docs.data", "docsite"),
         collection_url=collection_url,
         collection_install=collection_install,
+        referable_envvars=referable_envvars,
     )
     # Get the templates
     plugin_list_tmpl = env.get_template("list_of_plugins.rst.j2")
 
     collection_toplevel = os.path.join(dest_dir, "collections")
     flog.fields(
         toplevel=collection_toplevel, exists=os.path.isdir(collection_toplevel)
@@ -208,33 +214,38 @@
     flog.debug("Leave")
 
 
 async def output_environment_variables(
     dest_dir: str,
     env_variables: Mapping[str, EnvironmentVariableInfo],
     squash_hierarchy: bool = False,
+    referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Write environment variable Generate collection-level index pages for the collections.
 
     :arg dest_dir: The directory to place the documentation in.
     :arg env_variables: Mapping of environment variable names to environment variable information.
     :arg squash_hierarchy: If set to ``True``, no directory hierarchy will be used.
                            Undefined behavior if documentation for multiple collections are
                            created.
+    :kwarg referable_envvars: Optional set of environment variables that can be referenced.
     """
     flog = mlog.fields(func="write_environment_variables")
     flog.debug("Enter")
 
     if not squash_hierarchy:
         collection_toplevel = os.path.join(dest_dir, "collections")
     else:
         collection_toplevel = dest_dir
 
-    env = doc_environment(("antsibull_docs.data", "docsite"))
+    env = doc_environment(
+        ("antsibull_docs.data", "docsite"),
+        referable_envvars=referable_envvars,
+    )
     # Get the templates
     env_var_list_tmpl = env.get_template("list_of_env_variables.rst.j2")
 
     flog.fields(
         toplevel=collection_toplevel, exists=os.path.isdir(collection_toplevel)
     ).debug("collection_toplevel exists?")
     # This is only safe because we made sure that the top of the directory tree we're writing to
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/plugin_stubs.py` & `antsibull_docs-2.1.0/src/antsibull_docs/write_docs/plugin_stubs.py`

 * *Files 10% similar despite different names*

```diff
@@ -125,34 +125,37 @@
     dest_dir: str,
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     collection_metadata: Mapping[str, AnsibleCollectionMetadata],
     link_data: Mapping[str, CollectionLinks],
     squash_hierarchy: bool = False,
     for_official_docsite: bool = False,
+    referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Output rst files for each plugin stub.
 
     :arg stubs_info: Mapping of collection_name to Mapping of plugin_type to Mapping
         of plugin_name to routing information.
     :arg dest_dir: The directory to place the documentation in.
     :arg collection_metadata: Dictionary mapping collection names to collection metadata objects.
     :arg link_data: Dictionary mapping collection names to CollectionLinks.
     :arg squash_hierarchy: If set to ``True``, no directory hierarchy will be used.
                            Undefined behavior if documentation for multiple collections are
                            created.
     :kwarg for_official_docsite: Default False.  Set to True to use wording specific for the
         official docsite on docs.ansible.com.
+    :kwarg referable_envvars: Optional set of environment variables that can be referenced.
     """
     # Setup the jinja environment
     env = doc_environment(
         ("antsibull_docs.data", "docsite"),
         collection_url=collection_url,
         collection_install=collection_install,
+        referable_envvars=referable_envvars,
     )
     # Get the templates
     redirect_tmpl = env.get_template("plugin-redirect.rst.j2")
     tombstone_tmpl = env.get_template("plugin-tombstone.rst.j2")
 
     writers = []
     lib_ctx = app_context.lib_ctx.get()
```

### Comparing `antsibull_docs-2.0.0a2/src/antsibull_docs/write_docs/plugins.py` & `antsibull_docs-2.1.0/src/antsibull_docs/write_docs/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,14 +338,15 @@
     collection_url: CollectionNameTransformer,
     collection_install: CollectionNameTransformer,
     collection_metadata: Mapping[str, AnsibleCollectionMetadata],
     link_data: Mapping[str, CollectionLinks],
     squash_hierarchy: bool = False,
     use_html_blobs: bool = False,
     for_official_docsite: bool = False,
+    referable_envvars: set[str] | None = None,
 ) -> None:
     """
     Output rst files for each plugin.
 
     :arg collection_to_plugin_info: Mapping of collection_name to Mapping of plugin_type to Mapping
         of plugin_name to short_description.
     :arg plugin_info: Documentation information for all of the plugins.
@@ -357,20 +358,22 @@
     :arg squash_hierarchy: If set to ``True``, no directory hierarchy will be used.
                            Undefined behavior if documentation for multiple collections are
                            created.
     :arg use_html_blobs: If set to ``True``, will use HTML blobs for parameter and return value
                          tables instead of using RST tables.
     :kwarg for_official_docsite: Default False.  Set to True to use wording specific for the
         official docsite on docs.ansible.com.
+    :kwarg referable_envvars: Optional set of environment variables that can be referenced.
     """
     # Setup the jinja environment
     env = doc_environment(
         ("antsibull_docs.data", "docsite"),
         collection_url=collection_url,
         collection_install=collection_install,
+        referable_envvars=referable_envvars,
     )
     # Get the templates
     plugin_tmpl = env.get_template("plugin.rst.j2")
     role_tmpl = env.get_template("role.rst.j2")
     error_tmpl = env.get_template("plugin-error.rst.j2")
 
     writers = []
```

### Comparing `antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/__init__.py` & `antsibull_docs-2.1.0/src/sphinx_antsibull_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/antsibull-minimal.css` & `antsibull_docs-2.1.0/src/sphinx_antsibull_ext/antsibull-minimal.css`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/assets.py` & `antsibull_docs-2.1.0/src/sphinx_antsibull_ext/assets.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/roles.py` & `antsibull_docs-2.1.0/src/sphinx_antsibull_ext/roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,22 +250,72 @@
         entrypoint,
         rv_link,
         text,
     )
     return [nodes.literal(rawtext, text, *subnodes, classes=classes)], []
 
 
+# pylint:disable-next=unused-argument,dangerous-default-value
+def environment_variable(name, rawtext, text, lineno, inliner, options={}, content=[]):
+    """Format environment variable with possible assignment, without reference.
+
+    Returns 2 part tuple containing list of nodes to insert into the
+    document and a list of system messages.  Both are allowed to be
+    empty.
+
+    :param name: The role name used in the document.
+    :param rawtext: The entire markup snippet, with role.
+    :param text: The text marked with the role.
+    :param lineno: The line number where rawtext appears in the input.
+    :param inliner: The inliner instance that called us.
+    :param options: Directive options for customization.
+    :param content: The directive content for customization.
+    """
+    classes = ["xref", "std", "std-envvar"]
+    return [nodes.literal(rawtext, text, classes=classes)], []
+
+
+# pylint:disable-next=dangerous-default-value
+def environment_variable_reference(
+    name,  # pylint:disable=unused-argument
+    rawtext,
+    text,
+    lineno,  # pylint:disable=unused-argument
+    inliner,  # pylint:disable=unused-argument
+    options={},
+    content=[],
+):
+    # Extract the name of the environment variable
+    ref = text.replace("\x00", "").split("=", 1)[0].strip()
+
+    classes = ["xref", "std", "std-envvar"]
+    content = nodes.literal(rawtext, text, classes=classes)
+
+    options = {
+        "reftype": "envvar",
+        "refdomain": "std",
+        "refexplicit": True,
+        "refwarn": True,
+    }
+    refnode = addnodes.pending_xref(text, content, **options)
+    refnode["reftarget"] = ref
+
+    return [refnode], []
+
+
 ROLES = {
     "ansible-option-choices-entry": option_choice,
     "ansible-option-choices-entry-default": option_choice_default,
     "ansible-option-default": option_default,
     "ansible-rv-sample-value": return_value_sample,
     "ansopt": option_role,
     "ansval": value_role,
     "ansretval": return_value_role,
+    "ansenvvar": environment_variable,
+    "ansenvvarref": environment_variable_reference,
 }
 
 
 def setup_roles(app):
     """
     Setup roles for a Sphinx app object.
     """
```

### Comparing `antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/css/antsibull-minimal.scss` & `antsibull_docs-2.1.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/src/sphinx_antsibull_ext/css/build.sh` & `antsibull_docs-2.1.0/src/sphinx_antsibull_ext/css/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/stubs/rstcheck.pyi` & `antsibull_docs-2.1.0/stubs/rstcheck.pyi`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/stubs/rstcheck_core/config.pyi` & `antsibull_docs-2.1.0/stubs/rstcheck_core/config.pyi`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/validate-html.py` & `antsibull_docs-2.1.0/tests/validate-html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-all.json` & `antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns2.col.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9889509456961203%*

 * *Differences: {"'all'": "{'become': {'ns2.col.foo': {'doc': {'options': {'bar': {'deprecated': {'alternatives': "*

 * *          "'nothing\\nrelevant\\nI know of\\n', 'why': 'Just some other text.\\nThis one has more "*

 * *          "than one line though.\\nOne more.\\n'}}}, 'deprecated': OrderedDict([('alternatives', "*

 * *          '"I don\'t know\\nof any\\nalternative.\\n"), (\'removed_from_collection\', '*

 * *          "'ns2.col'), ('removed_in', '5.0.0'), ('why', 'Just some text.\\nThis one has more than "*

 * *          "one line.\\nAn […]*

```diff
@@ -1,27 +1,33 @@
 {
     "all": {
         "become": {
             "ns2.col.foo": {
                 "doc": {
                     "author": "Nobody (!UNKNOWN)",
                     "collection": "ns2.col",
+                    "deprecated": {
+                        "alternatives": "I don't know\nof any\nalternative.\n",
+                        "removed_from_collection": "ns2.col",
+                        "removed_in": "5.0.0",
+                        "why": "Just some text.\nThis one has more than one line.\nAnd one more.\n"
+                    },
                     "description": [
                         "This become plugin uses foo.",
                         "This is a second paragraph."
                     ],
                     "filename": "ansible_collections/ns2/col/plugins/become/foo.py",
                     "name": "foo",
                     "options": {
                         "bar": {
                             "deprecated": {
-                                "alternatives": "nothing",
+                                "alternatives": "nothing\nrelevant\nI know of\n",
                                 "collection_name": "ns2.col",
                                 "version": "4.0.0",
-                                "why": "Just some other text."
+                                "why": "Just some other text.\nThis one has more than one line though.\nOne more.\n"
                             },
                             "description": [
                                 "Bar. B(BAR!)",
                                 "Totally unrelated to O(become_user). Even with O(become_user=foo).",
                                 "Might not be compatible when O(become_user) is V(bar), though."
                             ],
                             "type": "str",
@@ -271,45 +277,61 @@
             }
         },
         "filter": {
             "ns2.col.bar": {
                 "doc": {
                     "collection": "ns2.col",
                     "description": [
-                        "Do some fooing."
+                        "Do some barring."
                     ],
-                    "filename": "ansible_collections/ns2/col/plugins/filter/foo.py",
-                    "name": "foo",
+                    "filename": "ansible_collections/ns2/col/plugins/filter/bar.yml",
+                    "name": "bar",
                     "options": {
                         "_input": {
                             "description": "The main input.",
                             "required": true,
-                            "type": "str"
+                            "type": "dict"
                         },
                         "bar": {
-                            "description": "Some bar.",
-                            "type": "string"
+                            "default": false,
+                            "description": "And some bar.",
+                            "type": "bool"
+                        },
+                        "baz": {
+                            "choices": {
+                                "a": "Whatever C(a) is.",
+                                "b": "What is C(b)? I don't know.",
+                                "cde": "This is some more unknown. There are rumors this is related to the alphabet.",
+                                "foo": [
+                                    "Our default value, the glorious C(foo).",
+                                    "Even has two paragraphs."
+                                ]
+                            },
+                            "default": "foo",
+                            "description": "Something else.",
+                            "type": "str"
                         },
                         "foo": {
                             "description": "Some foo.",
                             "elements": "dictionary",
                             "required": true,
                             "type": "list"
                         }
                     },
-                    "short_description": "The foo filter O(bar)",
-                    "version_added": "1.3.0",
+                    "positional": "foo, bar",
+                    "short_description": "The bar filter",
+                    "version_added": "2.0.0",
                     "version_added_collection": "ns2.col"
                 },
-                "examples": "\nsome_var: \"{{ 'foo' | ns2.col.foo }}\"\n",
+                "examples": "\n{'a': 1} | ns2.col.bar({'b': 2}, baz='cde')\n",
                 "metadata": null,
                 "return": {
                     "_value": {
                         "description": "The result.",
-                        "type": "str"
+                        "type": "dict"
                     }
                 }
             },
             "ns2.col.foo": {
                 "doc": {
                     "collection": "ns2.col",
                     "description": [
@@ -1044,249 +1066,14 @@
                         "elements": "str",
                         "type": "list"
                     }
                 }
             }
         },
         "module": {
-            "ns.col2.foo": {
-                "doc": {
-                    "attributes": {
-                        "check_mode": {
-                            "description": "Can run in check_mode and return changed status prediction without modifying target",
-                            "support": "full"
-                        },
-                        "diff_mode": {
-                            "description": "Will return details on what has changed (or possibly needs changing in check_mode), when in diff mode",
-                            "support": "full"
-                        },
-                        "platform": {
-                            "description": "Target OS/families that can be operated against",
-                            "details": [
-                                "The module M(boo) is not using an FQCN.",
-                                "Sometimes our markup is B(broken."
-                            ],
-                            "platforms": "posix",
-                            "support": "N/A"
-                        }
-                    },
-                    "author": [
-                        "Someone else (@ansible)"
-                    ],
-                    "collection": "ns.col2",
-                    "description": [
-                        "Does some foo on the remote host.",
-                        "A broken reference R(asdfasdfoobarTHISDOESNOTEXIST,asdfasdfoobarTHISDOESNOTEXIST).",
-                        "The option O(foo) exists, but O(foobar) does not.",
-                        "The return value RV(bar) exists, but RV(barbaz) does not.",
-                        "Again existing: O(ns.col2.foo#module:foo=1), RV(ns.col2.foo#module:bar=2)",
-                        "Again not existing: O(ns.col2.foo#module:foobar=1), RV(ns.col2.foo#module:barbaz=2)"
-                    ],
-                    "filename": "ansible_collections/ns/col2/plugins/modules/foo.py",
-                    "has_action": false,
-                    "module": "foo",
-                    "options": {
-                        "bar": {
-                            "description": [
-                                {
-                                    "A bar": [
-                                        "foo",
-                                        "bar",
-                                        "baz"
-                                    ]
-                                },
-                                true,
-                                42
-                            ],
-                            "type": "list of ints"
-                        },
-                        "foo": "The foo source.",
-                        "subfoo": {
-                            "bam": "baz",
-                            "description": "Some recursive foo.",
-                            "suboptions": {
-                                "foo": {
-                                    "description": [
-                                        "A sub foo.",
-                                        "Whatever.",
-                                        "Also required when I(subfoo) is specified when I(foo=bar) or C(baz)."
-                                    ],
-                                    "required": true,
-                                    "type": "str"
-                                }
-                            },
-                            "type": "dict"
-                        }
-                    },
-                    "requirements": "Foo.",
-                    "version_added": "foo",
-                    "version_added_collection": "ns.col2"
-                },
-                "examples": "\nThis is not YAML.\n",
-                "metadata": null,
-                "return": {
-                    "bar": {
-                        "description": "Some bar.",
-                        "returned": "success",
-                        "sample": "baz",
-                        "type": "string or so"
-                    },
-                    "baz": "baz!"
-                }
-            },
-            "ns.col2.foo2": {
-                "doc": {
-                    "attributes": {
-                        "check_mode": {
-                            "description": "Can run in check_mode and return changed status prediction without modifying target",
-                            "support": "full"
-                        },
-                        "diff_mode": {
-                            "description": "Will return details on what has changed (or possibly needs changing in check_mode), when in diff mode",
-                            "support": "full"
-                        },
-                        "platform": {
-                            "description": "Target OS/families that can be operated against",
-                            "details": [
-                                "The module M(boo) is not using an FQCN.",
-                                "Sometimes our markup is B(broken."
-                            ],
-                            "platforms": "posix",
-                            "support": "N/A"
-                        }
-                    },
-                    "author": [
-                        "Someone else (@ansible)"
-                    ],
-                    "collection": "ns.col2",
-                    "description": [
-                        "Does some foo on the remote host.",
-                        "A broken reference R(asdfasdfoobarTHISDOESNOTEXIST,asdfasdfoobarTHISDOESNOTEXIST).",
-                        "The option O(foo) exists, but O(foobar) does not.",
-                        "The return value RV(bar) exists, but RV(barbaz) does not.",
-                        "Again existing: O(ns.col2.foo#module:foo=1), RV(ns.col2.foo#module:bar=2)",
-                        "Again not existing: O(ns.col2.foo#module:foobar=1), RV(ns.col2.foo#module:barbaz=2)"
-                    ],
-                    "filename": "ansible_collections/ns/col2/plugins/modules/foo2.py",
-                    "has_action": false,
-                    "module": "foo2",
-                    "options": {
-                        "bar": {
-                            "description": [
-                                "Bar.",
-                                "Some O(broken markup)."
-                            ],
-                            "elements": "int",
-                            "type": "list"
-                        },
-                        "foo": {
-                            "description": "The foo source.",
-                            "type": "str"
-                        },
-                        "subfoo": {
-                            "description": "Some recursive foo.",
-                            "suboptions": {
-                                "foo": {
-                                    "description": [
-                                        "A sub foo.",
-                                        "Whatever.",
-                                        "Also required when I(subfoo) is specified when I(foo=bar) or C(baz).",
-                                        "RV(foobarbaz) does not exist."
-                                    ],
-                                    "required": true,
-                                    "type": "str"
-                                }
-                            },
-                            "type": "dict"
-                        }
-                    },
-                    "requirements": "Foo.",
-                    "short_description": "Foo two"
-                },
-                "examples": "\nname: This is YAML.\n",
-                "metadata": null,
-                "return": {
-                    "bar": {
-                        "description": "Some bar.",
-                        "returned": "success",
-                        "sample": "baz",
-                        "type": "string"
-                    }
-                }
-            },
-            "ns.col2.foo3": {
-                "doc": {
-                    "attributes": {
-                        "check_mode": {
-                            "description": "Can run in check_mode and return changed status prediction without modifying target",
-                            "support": "full"
-                        },
-                        "diff_mode": {
-                            "description": "Will return details on what has changed (or possibly needs changing in check_mode), when in diff mode",
-                            "support": "full"
-                        },
-                        "platform": {
-                            "description": "Target OS/families that can be operated against",
-                            "platforms": "posix",
-                            "support": "N/A"
-                        }
-                    },
-                    "author": [
-                        "Someone else (@ansible)"
-                    ],
-                    "collection": "ns.col2",
-                    "description": [
-                        "Does some foo on the remote host."
-                    ],
-                    "filename": "ansible_collections/ns/col2/plugins/modules/foo3.py",
-                    "has_action": false,
-                    "module": "foo3",
-                    "options": {
-                        "bar": {
-                            "description": [
-                                "Bar."
-                            ],
-                            "elements": "int",
-                            "type": "list"
-                        },
-                        "foo": {
-                            "description": "The foo source.",
-                            "type": "str"
-                        },
-                        "subfoo": {
-                            "description": "Some recursive foo.",
-                            "suboptions": {
-                                "foo": {
-                                    "description": [
-                                        "A sub foo.",
-                                        "Whatever.",
-                                        "Also required when I(subfoo) is specified when I(foo=bar) or C(baz)."
-                                    ],
-                                    "required": true,
-                                    "type": "str"
-                                }
-                            },
-                            "type": "dict"
-                        }
-                    },
-                    "requirements": "Foo.",
-                    "short_description": "Foo III"
-                },
-                "examples": "\nThis is not YAML.\n",
-                "metadata": null,
-                "return": {
-                    "bar": {
-                        "description": "Some bar.",
-                        "returned": "success",
-                        "sample": "baz",
-                        "type": "string or so"
-                    },
-                    "baz": "baz!"
-                }
-            },
             "ns2.col.foo": {
                 "doc": {
                     "attributes": {
                         "action_group": {
                             "description": "Use C(group/ns2.col.foo_group) in C(module_defaults) to set defaults for this module.",
                             "membership": [
                                 "ns2.col.foo_group"
@@ -1310,15 +1097,16 @@
                     "author": [
                         "Ansible Core Team",
                         "Someone else (@ansible)"
                     ],
                     "collection": "ns2.col",
                     "description": [
                         "Does some foo on the remote host.",
-                        "Whether foo is magic or not has not yet been determined."
+                        "Whether foo is magic or not has not yet been determined.",
+                        "E(FOOBAR1), E(FOOBAR2), E(FOOBAR3), E(FOOBAR4)."
                     ],
                     "filename": "ansible_collections/ns2/col/plugins/modules/foo.py",
                     "has_action": false,
                     "module": "foo",
                     "options": {
                         "bar": {
                             "aliases": [
@@ -1508,122 +1296,14 @@
                             "Do not confuse with O(bar)."
                         ],
                         "returned": "success",
                         "sample": "baz",
                         "type": "str"
                     }
                 }
-            },
-            "ns2.flatcol.foo": {
-                "doc": {
-                    "author": [
-                        "Ansible Core Team",
-                        "Someone else (@ansible)"
-                    ],
-                    "collection": "ns2.flatcol",
-                    "description": [
-                        "Does some foo on the remote host.",
-                        "Whether foo is magic or not has not yet been determined."
-                    ],
-                    "filename": "ansible_collections/ns2/flatcol/plugins/modules/foo.py",
-                    "has_action": false,
-                    "module": "foo",
-                    "options": {
-                        "bar": {
-                            "aliases": [
-                                "baz"
-                            ],
-                            "description": [
-                                "A bar.",
-                                "Independent from O(foo).",
-                                "Do not confuse with RV(bar)."
-                            ],
-                            "elements": "int",
-                            "type": "list"
-                        },
-                        "foo": {
-                            "description": "The foo source.",
-                            "required": true,
-                            "type": "str"
-                        },
-                        "subfoo": {
-                            "description": "Some recursive foo.",
-                            "suboptions": {
-                                "foo": {
-                                    "description": [
-                                        "A sub foo.",
-                                        "Whatever.",
-                                        "Also required when O(subfoo) is specified when O(foo=bar) or V(baz)."
-                                    ],
-                                    "required": true,
-                                    "type": "str"
-                                }
-                            },
-                            "type": "dict",
-                            "version_added": "2.0.0",
-                            "version_added_collection": "ns2.flatcol"
-                        }
-                    },
-                    "short_description": "Do some foo O(bar)",
-                    "version_added": "2.0.0",
-                    "version_added_collection": "ns2.flatcol"
-                },
-                "examples": "\n- name: Do some foo\n  ns2.flatcol.foo:\n    foo: '{{ foo }}'\n    bar:\n      - 1\n      - 2\n      - 3\n    subfoo:\n      foo: hoo!\n",
-                "metadata": null,
-                "return": {
-                    "bar": {
-                        "description": [
-                            "Some bar.",
-                            "Referencing myself as RV(bar).",
-                            "Do not confuse with O(bar)."
-                        ],
-                        "returned": "success",
-                        "sample": "baz",
-                        "type": "str"
-                    }
-                }
-            },
-            "ns2.flatcol.sub.foo2": {
-                "doc": {
-                    "author": [
-                        "Another one (@ansible-community)"
-                    ],
-                    "collection": "ns2.flatcol",
-                    "description": [
-                        "Foo bar.",
-                        "See O(ns2.flatcol.foo#role:main:foo_param_1) for a random role parameter reference. And O(ns2.flatcol.foo#role:main:foo_param_2=42) for one with a value."
-                    ],
-                    "filename": "ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py",
-                    "has_action": false,
-                    "module": "foo2",
-                    "options": {
-                        "bar": {
-                            "description": [
-                                "Some bar.",
-                                "See O(ns2.flatcol.foo#role:main:foo_param_1) for a random role parameter reference. And O(ns2.flatcol.foo#role:main:foo_param_2=42) for one with a value."
-                            ],
-                            "type": "str"
-                        }
-                    },
-                    "short_description": "Another foo"
-                },
-                "examples": "\n- name: Do some foo\n  ns2.flatcol.foo2:\n    bar: foo\n",
-                "metadata": null,
-                "return": {
-                    "bar": {
-                        "description": [
-                            "Some bar.",
-                            "Referencing myself as RV(bar).",
-                            "Do not confuse with O(bar)."
-                        ],
-                        "returned": "success",
-                        "sample": "baz",
-                        "type": "str"
-                    }
-                }
             }
         },
         "netconf": {},
         "role": {
             "ns2.col.foo": {
                 "collection": "ns2.col",
                 "entry_points": {
@@ -1633,14 +1313,19 @@
                                 "description": "Can run in check_mode and return changed status prediction without modifying target",
                                 "support": "full"
                             }
                         },
                         "author": [
                             "Felix Fontein (@felixfontein)"
                         ],
+                        "deprecated": {
+                            "alternatives": "I don't know\nof any\nalternative.\n",
+                            "removed_in": "5.0.0",
+                            "why": "Just some text.\nThis one has more than one line.\nAnd one more.\n"
+                        },
                         "description": [
                             "This is the foo role.",
                             "If you set O(foo_param_1) while O(foo_param_2=3), this might behave funny."
                         ],
                         "options": {
                             "foo_param_1": {
                                 "description": [
@@ -1736,39 +1421,37 @@
                 "metadata": null,
                 "return": null
             }
         },
         "test": {
             "ns2.col.bar": {
                 "doc": {
-                    "author": "Nobody",
+                    "aliases": [
+                        "is_bar"
+                    ],
+                    "author": "Ansible Core",
                     "collection": "ns2.col",
                     "description": [
-                        "Check whether the input dictionary is a foo."
+                        "Check whether a path is a bar."
                     ],
-                    "filename": "ansible_collections/ns2/col/plugins/test/foo.py",
-                    "name": "foo",
+                    "filename": "ansible_collections/ns2/col/plugins/test/bar.yml",
+                    "name": "bar",
                     "options": {
                         "_input": {
-                            "description": "Something to test.",
-                            "required": true,
-                            "type": "dictionary"
-                        },
-                        "bar": {
-                            "description": "Foo bar.",
-                            "type": "string"
+                            "description": "A path.",
+                            "type": "path"
                         }
                     },
-                    "short_description": "Is something a foo O(bar)"
+                    "short_description": "Is something a bar"
                 },
-                "examples": "\nsome_var: \"{{ {'a': 1} is ns2.col.foo }}\"\n",
+                "examples": "is_path_bar: \"{{ '/etc/hosts' is ns2.col.bar }}}\"\n",
                 "metadata": null,
                 "return": {
                     "_value": {
-                        "description": "Whether the input is a foo.",
+                        "description": "Returns C(true) if the path is a bar, C(false) if it is not a bar.",
                         "type": "boolean"
                     }
                 }
             },
             "ns2.col.foo": {
                 "doc": {
                     "author": "Nobody",
@@ -1798,39 +1481,37 @@
                         "description": "Whether the input is a foo.",
                         "type": "boolean"
                     }
                 }
             },
             "ns2.col.is_bar": {
                 "doc": {
-                    "author": "Nobody",
+                    "aliases": [
+                        "is_bar"
+                    ],
+                    "author": "Ansible Core",
                     "collection": "ns2.col",
                     "description": [
-                        "Check whether the input dictionary is a foo."
+                        "Check whether a path is a bar."
                     ],
-                    "filename": "ansible_collections/ns2/col/plugins/test/foo.py",
-                    "name": "foo",
+                    "filename": "ansible_collections/ns2/col/plugins/test/is_bar.yml",
+                    "name": "bar",
                     "options": {
                         "_input": {
-                            "description": "Something to test.",
-                            "required": true,
-                            "type": "dictionary"
-                        },
-                        "bar": {
-                            "description": "Foo bar.",
-                            "type": "string"
+                            "description": "A path.",
+                            "type": "path"
                         }
                     },
-                    "short_description": "Is something a foo O(bar)"
+                    "short_description": "Is something a bar"
                 },
-                "examples": "\nsome_var: \"{{ {'a': 1} is ns2.col.foo }}\"\n",
+                "examples": "is_path_bar: \"{{ '/etc/hosts' is ns2.col.bar }}}\"\n",
                 "metadata": null,
                 "return": {
                     "_value": {
-                        "description": "Whether the input is a foo.",
+                        "description": "Returns C(true) if the path is a bar, C(false) if it is not a bar.",
                         "type": "boolean"
                     }
                 }
             }
         },
         "vars": {
             "ns2.col.foo": {
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns.col1.json` & `antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns.col1.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns.col2.json` & `antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns.col2.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963235294117647%*

 * *Differences: {"'all'": "{'module': {'ns.col2.foo4': OrderedDict([('doc', OrderedDict([('author', ['Nobody "*

 * *          "(@ansible)']), ('collection', 'ns.col2'), ('description', []), ('filename', "*

 * *          "'ansible_collections/ns/col2/plugins/modules/foo4.py'), ('has_action', False), "*

 * *          "('module', 'foo4'), ('options', OrderedDict([('existing', OrderedDict([('description', "*

 * *          "['M(ansible.builtin.service)', 'P(ansible.builtin.pipe#lookup)', "*

 * *          "'O(ansible.builtin.file#module:state)', 'RV(ans […]*

```diff
@@ -874,14 +874,91 @@
                         "description": "Some bar.",
                         "returned": "success",
                         "sample": "baz",
                         "type": "string or so"
                     },
                     "baz": "baz!"
                 }
+            },
+            "ns.col2.foo4": {
+                "doc": {
+                    "author": [
+                        "Nobody (@ansible)"
+                    ],
+                    "collection": "ns.col2",
+                    "description": [],
+                    "filename": "ansible_collections/ns/col2/plugins/modules/foo4.py",
+                    "has_action": false,
+                    "module": "foo4",
+                    "options": {
+                        "existing": {
+                            "description": [
+                                "M(ansible.builtin.service)",
+                                "P(ansible.builtin.pipe#lookup)",
+                                "O(ansible.builtin.file#module:state)",
+                                "RV(ansible.builtin.stat#module:stat.exists)",
+                                "M(ns2.flatcol.foo)",
+                                "P(ns2.flatcol.sub.foo2#module)",
+                                "O(ns2.flatcol.foo#module:subbaz.bam)",
+                                "RV(ns2.flatcol.sub.foo2#module:bar)",
+                                "M(ns2.col.foo2)",
+                                "P(ns2.col.foo#lookup)",
+                                "O(ns2.col.bar#filter:foo[-1])",
+                                "RV(ns2.col.bar#test:_value)",
+                                "M(ns.col2.foo2)",
+                                "P(ns.col2.foo2#module)",
+                                "O(ns.col2.foo2#module:subfoo.foo)",
+                                "RV(ns.col2.foo2#module:bar)",
+                                "M(ext.col.foo)",
+                                "P(ext.col.bar#lookup)",
+                                "O(ext.col.foo#module:foo[len(foo\\)].bar)",
+                                "RV(ext.col.foo#module:baz[])"
+                            ]
+                        },
+                        "not_existing": {
+                            "description": [
+                                "M(ansible.builtin.foobar)",
+                                "P(ansible.builtin.bazbam#lookup)",
+                                "O(ansible.builtin.file#module:foobarbaz)",
+                                "RV(ansible.builtin.stat#module:baz.bam[])",
+                                "O(ansible.builtin.foobar#module:state)",
+                                "RV(ansible.builtin.bazbam#module:stat.exists)",
+                                "M(ns2.flatcol.foobarbaz)",
+                                "P(ns2.flatcol.sub.bazbam#module)",
+                                "O(ns2.flatcol.foo#module:foofoofoobar)",
+                                "RV(ns2.flatcol.sub.foo2#module:bazbarbam)",
+                                "O(ns2.flatcol.foobar#module:subbaz.bam)",
+                                "RV(ns2.flatcol.sub.bazbam#module:bar)",
+                                "M(ns2.col.joo)",
+                                "P(ns2.col.joo#lookup)",
+                                "O(ns2.col.bar#filter:jooo)",
+                                "RV(ns2.col.bar#test:booo)",
+                                "O(ns2.col.joo#filter:foo[-1])",
+                                "RV(ns2.col.joo#test:_value)",
+                                "M(ns.col2.foobarbaz)",
+                                "P(ns.col2.foobarbam#filter)",
+                                "O(ns.col2.foo2#module:barbazbam.foo)",
+                                "RV(ns.col2.foo2#module:bambazbar)",
+                                "O(ns.col2.foofoo#test:subfoo.foo)",
+                                "RV(ns.col2.foofoo#lookup:baz)",
+                                "M(ext.col.notthere)",
+                                "P(ext.col.notthere#lookup)",
+                                "O(ext.col.foo#module:foo[len(foo\\)].notthere)",
+                                "O(ext.col.foo#module:notthere[len(notthere\\)].bar)",
+                                "RV(ext.col.foo#module:notthere[])",
+                                "O(ext.col.notthere#module:foo[len(foo\\)].bar)",
+                                "RV(ext.col.notthere#module:baz[])"
+                            ]
+                        }
+                    },
+                    "short_description": "Markup reference linting test"
+                },
+                "examples": null,
+                "metadata": null,
+                "return": null
             }
         },
         "netconf": {},
         "role": {},
         "shell": {},
         "strategy": {},
         "test": {},
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/ansible-doc-cache-ns2.flatcol.json` & `antsibull_docs-2.1.0/tests/functional/ansible-doc-cache-ns2.flatcol.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993138531454%*

 * *Differences: {"'all'": "{'module': {'ns2.flatcol.foo': {'doc': {'options': {'subfoo': {'suboptions': {'foo': "*

 * *          "{'description': {insert: [(3, 'Note that O(subfoo.foo) is the same as O(subbaz.foo), "*

 * *          "O(subbaz.bam), and O(subfoo.bam).'), (4, 'E(FOOBAR1), E(FOOBAR2), E(FOOBAR3), "*

 * *          "E(FOOBAR4).')]}, 'aliases': ['bam']}}, 'aliases': ['subbaz']}}}}}}"}*

```diff
@@ -673,21 +673,29 @@
                         },
                         "foo": {
                             "description": "The foo source.",
                             "required": true,
                             "type": "str"
                         },
                         "subfoo": {
+                            "aliases": [
+                                "subbaz"
+                            ],
                             "description": "Some recursive foo.",
                             "suboptions": {
                                 "foo": {
+                                    "aliases": [
+                                        "bam"
+                                    ],
                                     "description": [
                                         "A sub foo.",
                                         "Whatever.",
-                                        "Also required when O(subfoo) is specified when O(foo=bar) or V(baz)."
+                                        "Also required when O(subfoo) is specified when O(foo=bar) or V(baz).",
+                                        "Note that O(subfoo.foo) is the same as O(subbaz.foo), O(subbaz.bam), and O(subfoo.bam).",
+                                        "E(FOOBAR1), E(FOOBAR2), E(FOOBAR3), E(FOOBAR4)."
                                     ],
                                     "required": true,
                                     "type": "str"
                                 }
                             },
                             "type": "dict",
                             "version_added": "2.0.0",
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/ansible-version.output` & `antsibull_docs-2.1.0/tests/functional/ansible-version.output`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ansible [core 2.16.0.dev0] (devel abc58c026b) last updated 2023/04/25 07:58:13 (GMT +200)
+ansible [core 2.16.0.dev0] (devel 73e04ef2d6) last updated 2023/06/13 23:00:13 (GMT +200)
   config file = None
   configured module search path = ['<<<<<HOME>>>>>/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
   ansible python module location = <<<<<ANSIBLE>>>>>
   ansible collection location = <<<<<COLLECTIONS>>>>>
   executable location = <<<<<HOME>>>>>/.local/bin/ansible
-  python version = 3.10.10 (main, Mar  5 2023, 22:26:53) [GCC 12.2.1 20230201] (/usr/bin/python)
+  python version = 3.11.3 (main, Jun  5 2023, 09:32:32) [GCC 13.1.1 20230429] (/usr/bin/python)
   jinja version = 3.1.2
   libyaml = True
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/build-docs-baseline.sh` & `antsibull_docs-2.1.0/tests/functional/build-docs-baseline.sh`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     mkdir -p "${DEST}"
     ANSIBLE_COLLECTIONS_PATHS= ANSIBLE_COLLECTIONS_PATH=collections/ antsibull-docs collection --dest-dir "${DEST}" --use-current "$@" 2>&1 | (
         set +e
         grep -v "ERROR:antsibull:func=create_plugin_rst:mod=antsibull_docs.write_docs.plugins:nonfatal_errors="
         set -e
     )
 
-    rstcheck --report-level warning --ignore-roles ansible-option-default,ansible-rv-sample-value,ansopt,ansval,ansretval -r "${DEST}" 2>&1 | (
+    rstcheck --report-level warning --ignore-roles ansible-option-default,ansible-rv-sample-value,ansopt,ansval,ansretval,ansible-option-choices-entry-default,ansible-option-choices-entry,ansenvvar,ansenvvarref -r "${DEST}" 2>&1 | (
         set +e
         grep -v "CRITICAL:rstcheck_core.checker:An \`AttributeError\` error occured."
         set -e
     )
 }
 
 
@@ -49,7 +49,13 @@
 ANSIBLE_COLLECTIONS_PATHS= ANSIBLE_COLLECTIONS_PATH=collections/ ansible --version | sed -e "s|${PWD}/collections|<<<<<COLLECTIONS>>>>>|g" | sed -e "s|${HOME}|<<<<<HOME>>>>>|g" | sed -E "s|(ansible python module location = ).*|\\1<<<<<ANSIBLE>>>>>|g" > ansible-version.output
 
 make_ansible_doc_extract all
 make_ansible_doc_extract ns.col1 ns.col1
 make_ansible_doc_extract ns.col2 ns.col2
 make_ansible_doc_extract ns2.col ns2.col
 make_ansible_doc_extract ns2.flatcol ns2.flatcol
+
+echo "Build extended ansible-galaxy collection list output cache"
+ANSIBLE_COLLECTIONS_PATHS= ANSIBLE_COLLECTIONS_PATH=collections/:other-collections/ ansible-galaxy collection list --format json | python sanitize-ansible-galaxy-list.py > "ansible-galaxy-cache-all-others.json"
+
+echo "Build extended ansible-doc --metadata-dump --no-fail-on-errors output cache"
+ANSIBLE_COLLECTIONS_PATHS= ANSIBLE_COLLECTIONS_PATH=collections/:other-collections/ ansible-doc --metadata-dump --no-fail-on-errors | python sanitize-ansible-doc-dump.py > "ansible-doc-cache-all-others.json"
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/build-sphinx-init-baseline.sh` & `antsibull_docs-2.1.0/tests/functional/build-sphinx-init-baseline.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/sanitize-ansible-doc-dump.py` & `antsibull_docs-2.1.0/tests/functional/sanitize-ansible-doc-dump.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 import json
 import os
 import sys
 
 import ansible
 
 root = os.path.join(os.getcwd(), "collections")
+other_root = os.path.join(os.getcwd(), "other-collections")
 ansible_root = os.path.dirname(ansible.__file__)
 data = json.load(sys.stdin)
 for plugin_type, plugins in data["all"].items():
     for plugin_fqcn, plugin_data in list(plugins.items()):
-        if plugin_fqcn.startswith("ansible.builtin."):
-            del plugins[plugin_fqcn]
         for doc_key, key in [
             ("doc", "filename"),
             ("", "path"),
         ]:
             doc = plugin_data
             if doc_key:
                 if doc_key not in doc:
                     continue
                 doc = doc[doc_key]
             if key in doc:
                 rel_root = os.path.relpath(doc[key], root)
                 rel_ansible = os.path.relpath(doc[key], ansible_root)
-                if not rel_root.startswith("."):
-                    doc[key] = os.path.join(rel_root)
+                if not rel_root.startswith(".") or rel_root.startswith(
+                    "../other-collections/"
+                ):
+                    doc[key] = rel_root
                 elif not rel_ansible.startswith("."):
                     doc[key] = os.path.join("/ansible", rel_ansible)
                 else:
                     raise Exception(f"Cannot sanitize {doc[key]}")
 json.dump(data, sys.stdout, indent=1, sort_keys=True)
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/sanitize-ansible-galaxy-list.py` & `antsibull_docs-2.1.0/tests/functional/sanitize-ansible-galaxy-list.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from __future__ import annotations
 
 import json
 import os
 import sys
 
 root = os.path.join(os.getcwd(), "collections")
+other_root = os.path.join(os.getcwd(), "other-collections")
 data = json.load(sys.stdin)
 result = {}
 for path, collections in data.items():
     rel_root = os.path.relpath(path, root)
-    if rel_root.startswith("."):
+    if rel_root.startswith(".") and not rel_root.startswith("../other-collections/"):
         raise Exception(f"Cannot sanitize {doc[key]}")
     result[rel_root] = collections
 json.dump(result, sys.stdout, indent=1, sort_keys=True)
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/test_docs_baseline.py` & `antsibull_docs-2.1.0/tests/functional/test_docs_baseline.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/test_sphinx_init_baseline.py` & `antsibull_docs-2.1.0/tests/functional/test_sphinx_init_baseline.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             "--no-indexes",
             "--no-breadcrumbs",
             "--use-html-blobs",
             "--squash-hierarchy",
             "--lenient",
             "--fail-on-error",
             "--index-rst-source",
-            "tests/functional/test.rst",
+            os.path.join(os.path.dirname(__file__), "test.rst"),
             "--intersphinx",
             "identifier:https://server/path",
             "--intersphinx",
             "foo:https://bar/baz",
             "--sphinx-theme",
             "another-theme",
         ],
@@ -130,15 +130,15 @@
     if differences:
         print(f"Found {differences} differences.")
     assert differences == 0
 
 
 @pytest.mark.parametrize("arguments, directory", TEST_CASES)
 def test_baseline(arguments, directory, tmp_path):
-    tests_root = os.path.join("tests", "functional")
+    tests_root = os.path.dirname(__file__)
 
     # Re-build baseline
     command = ["antsibull-docs", "sphinx-init", "--dest-dir", str(tmp_path)] + arguments
     stdout = io.StringIO()
     with redirect_stdout(stdout):
         rc = run(command)
     stdout = stdout.getvalue().splitlines()
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/environment_variables.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/index_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/index_module.rst`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ns.col2
 -------
 
 * :ref:`ns.col2.foo <ansible_collections.ns.col2.foo_module>` -- 
 * :ref:`ns.col2.foo2 <ansible_collections.ns.col2.foo2_module>` -- Foo two
 * :ref:`ns.col2.foo3 <ansible_collections.ns.col2.foo3_module>` -- Foo III
+* :ref:`ns.col2.foo4 <ansible_collections.ns.col2.foo4_module>` -- Markup reference linting test
 
 ns2.col
 -------
 
 * :ref:`ns2.col.foo <ansible_collections.ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
 * :ref:`ns2.col.foo2 <ansible_collections.ns2.col.foo2_module>` -- Another foo
 * :ref:`ns2.col.sub.foo3 <ansible_collections.ns2.col.sub.foo3_module>` -- A sub-foo
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns/col2/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+:orphan:
 
 
 .. _plugins_in_ns.col2:
 
 Ns.Col2
 =======
 
@@ -39,21 +40,14 @@
 
 Modules
 ~~~~~~~
 
 * :ref:`foo module <ansible_collections.ns.col2.foo_module>` -- 
 * :ref:`foo2 module <ansible_collections.ns.col2.foo2_module>` -- Foo two
 * :ref:`foo3 module <ansible_collections.ns.col2.foo3_module>` -- Foo III
-
-.. toctree::
-    :maxdepth: 1
-    :hidden:
-
-    foo_module
-    foo2_module
-    foo3_module
+* :ref:`foo4 module <ansible_collections.ns.col2.foo4_module>` -- Markup reference linting test
 
 
 
 .. seealso::
 
     List of :ref:`collections <list_of_collections>` with docs hosted here.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. contents::
    :local:
    :depth: 1
 
 .. Deprecated
 
+DEPRECATED
+----------
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 --------
 
 .. Description
 
 - This become plugin uses foo.
@@ -115,16 +126,22 @@
       :ansible-option-versionadded:`added in ns2.col 1.2.0`
 
 
 
       Removed in: version 4.0.0
 
       Why: Just some other text.
+      This one has more than one line though.
+      One more.
+
 
       Alternative: nothing
+      relevant
+      I know of
+
 
 
 
 
       .. raw:: html
 
         </div>
@@ -335,14 +352,23 @@
 
 
 .. Return values
 
 
 ..  Status (Presently only deprecated)
 
+Status
+------
+
+.. Deprecated note
+
+- This become will be removed in version 5.0.0.
+  *[deprecated]*
+- For more information see `DEPRECATED`_.
+
 
 .. Authors
 
 Authors
 ~~~~~~~
 
 - Nobody
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
+- \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. rst-class:: ansible-version-added
 
 New in ns2.col 0.2.0
 
 .. Deprecated
 
+DEPRECATED
+^^^^^^^^^^
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 ^^^^^^^^
 
 .. Description
 
 - This is the foo role.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -146,20 +146,22 @@
 
     foo_connection
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
+* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
 * :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
+    bar_filter
     foo_filter
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
 * :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
@@ -206,20 +208,22 @@
 
     foo_strategy
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
+* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
 * :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
+    bar_test
     foo_test
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
 * :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\
```

#### html2text {}

```diff
@@ -30,30 +30,32 @@
 toctree:: :maxdepth: 1 :hidden: foo_callback Cliconf Plugins ~~~~~~~~~~~~~~~ *
 :ref:`foo cliconf
 ns2.col.foo_cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :
 hidden: foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ref:`foo
 connection
 ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
 bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins
-~~~~~~~~~~~~~~ * :ref:`foo filter
+~~~~~~~~~~~~~~ * :ref:`bar filter
+ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
 ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_filter Inventory Plugins ~~~~~~~~~~~~~~~~~
-* :ref:`foo inventory
+toctree:: :maxdepth: 1 :hidden: bar_filter foo_filter Inventory Plugins
+~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
 ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
 bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins
 ~~~~~~~~~~~~~~ * :ref:`foo lookup
 ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :ref:
 `foo shell
 ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :
 ref:`foo strategy
 ns2.col.foo_strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :
-hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`foo test
+hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`bar test
+ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
 ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_test Vars Plugins ~~~~~~~~~~~~ * :ref:`foo
-vars
+toctree:: :maxdepth: 1 :hidden: bar_test foo_test Vars Plugins ~~~~~~~~~~~~ * :
+ref:`foo vars
 ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
 maxdepth: 1 :hidden: foo_vars Role Index ---------- These are the roles in the
 ns2.col collection: * :ref:`foo role
 ns2.col.foo_role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
 seealso:: List of :ref:`collections ` with docs hosted here.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst`

 * *Files 7% similar despite different names*

```diff
@@ -173,27 +173,33 @@
 
         </div>
 
   * - .. raw:: html
 
         <div class="ansible-option-cell">
         <div class="ansibleOptionAnchor" id="parameter-subfoo"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subbaz"></div>
 
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz:
       .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo:
 
       .. rst-class:: ansible-option-title
 
       **subfoo**
 
       .. raw:: html
 
         <a class="ansibleOptionLink" href="#parameter-subfoo" title="Permalink to this option"></a>
 
       .. rst-class:: ansible-option-type-line
 
+      :ansible-option-aliases:`aliases: subbaz`
+
+      .. rst-class:: ansible-option-type-line
+
       :ansible-option-type:`dictionary`
 
       :ansible-option-versionadded:`added in ns2.flatcol 2.0.0`
 
 
       .. raw:: html
 
@@ -210,27 +216,37 @@
 
         </div>
     
   * - .. raw:: html
 
         <div class="ansible-option-indent"></div><div class="ansible-option-cell">
         <div class="ansibleOptionAnchor" id="parameter-subfoo/foo"></div>
-
+        <div class="ansibleOptionAnchor" id="parameter-subbaz/foo"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subfoo/bam"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subbaz/bam"></div>
+
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz/bam:
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz/foo:
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo/bam:
       .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo/foo:
 
       .. rst-class:: ansible-option-title
 
       **foo**
 
       .. raw:: html
 
         <a class="ansibleOptionLink" href="#parameter-subfoo/foo" title="Permalink to this option"></a>
 
       .. rst-class:: ansible-option-type-line
 
+      :ansible-option-aliases:`aliases: bam`
+
+      .. rst-class:: ansible-option-type-line
+
       :ansible-option-type:`string` / :ansible-option-required:`required`
 
       .. raw:: html
 
         </div>
 
     - .. raw:: html
@@ -239,14 +255,18 @@
 
       A sub foo.
 
       Whatever.
 
       Also required when \ :ansopt:`ns2.flatcol.foo#module:subfoo`\  is specified when \ :ansopt:`ns2.flatcol.foo#module:foo=bar`\  or \ :ansval:`baz`\ .
 
+      Note that \ :ansopt:`ns2.flatcol.foo#module:subfoo.foo`\  is the same as \ :ansopt:`ns2.flatcol.foo#module:subbaz.foo`\ , \ :ansopt:`ns2.flatcol.foo#module:subbaz.bam`\ , and \ :ansopt:`ns2.flatcol.foo#module:subfoo.bam`\ .
+
+      \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
+
 
       .. raw:: html
 
         </div>
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-default/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 ns.col2
 -------
 
 * :ref:`ns.col2.foo <ansible_collections.ns.col2.foo_module>` -- 
 * :ref:`ns.col2.foo2 <ansible_collections.ns.col2.foo2_module>` -- Foo two
 * :ref:`ns.col2.foo3 <ansible_collections.ns.col2.foo3_module>` -- Foo III
+* :ref:`ns.col2.foo4 <ansible_collections.ns.col2.foo4_module>` -- Markup reference linting test
 
 ns2.col
 -------
 
 * :ref:`ns2.col.foo <ansible_collections.ns2.col.foo_module>` -- Do some foo \ :ansopt:`ns2.col.foo#module:bar`\ 
 * :ref:`ns2.col.foo2 <ansible_collections.ns2.col.foo2_module>` -- Another foo
 * :ref:`ns2.col.sub.foo3 <ansible_collections.ns2.col.sub.foo3_module>` -- A sub-foo
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 
-:orphan:
 
 
-.. _plugins_in_ns.col2:
+.. _plugins_in_ns2.flatcol:
 
-Ns.Col2
-=======
+Ns2.Flatcol
+===========
 
-Collection version 0.0.1
 
 .. contents::
    :local:
    :depth: 1
 
 Description
 -----------
 
 
 **Author:**
 
 * Ansible (https://github.com/ansible)
 
-**Supported ansible-core versions:**
-
-* newer than 2.11.0
 
 
 
 
 .. toctree::
     :maxdepth: 1
 
 
 Plugin Index
 ------------
 
-These are the plugins in the ns.col2 collection:
+These are the plugins in the ns2.flatcol collection:
 
 
 Modules
 ~~~~~~~
 
-* :ref:`foo module <ansible_collections.ns.col2.foo_module>` -- 
-* :ref:`foo2 module <ansible_collections.ns.col2.foo2_module>` -- Foo two
-* :ref:`foo3 module <ansible_collections.ns.col2.foo3_module>` -- Foo III
+* :ref:`foo module <ansible_collections.ns2.flatcol.foo_module>` -- Do some foo \ :ansopt:`ns2.flatcol.foo#module:bar`\ 
+* :ref:`foo2 module <ansible_collections.ns2.flatcol.foo2_module>` -- Another foo
+
+.. toctree::
+    :maxdepth: 1
+    :hidden:
+
+    foo_module
+    foo2_module
 
 
 
 .. seealso::
 
     List of :ref:`collections <list_of_collections>` with docs hosted here.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. contents::
    :local:
    :depth: 1
 
 .. Deprecated
 
+DEPRECATED
+----------
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 --------
 
 .. Description
 
 - This become plugin uses foo.
@@ -115,16 +126,22 @@
       :ansible-option-versionadded:`added in ns2.col 1.2.0`
 
 
 
       Removed in: version 4.0.0
 
       Why: Just some other text.
+      This one has more than one line though.
+      One more.
+
 
       Alternative: nothing
+      relevant
+      I know of
+
 
 
 
 
       .. raw:: html
 
         </div>
@@ -335,14 +352,23 @@
 
 
 .. Return values
 
 
 ..  Status (Presently only deprecated)
 
+Status
+------
+
+.. Deprecated note
+
+- This become will be removed in version 5.0.0.
+  *[deprecated]*
+- For more information see `DEPRECATED`_.
+
 
 .. Authors
 
 Authors
 ~~~~~~~
 
 - Nobody
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
+- \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. rst-class:: ansible-version-added
 
 New in ns2.col 0.2.0
 
 .. Deprecated
 
+DEPRECATED
+^^^^^^^^^^
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 ^^^^^^^^
 
 .. Description
 
 - This is the foo role.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 
 * :ref:`foo connection <ansible_collections.ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:bar`\ 
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
+* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
 * :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
 * :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
@@ -139,14 +140,15 @@
 
 * :ref:`foo strategy <ansible_collections.ns2.col.foo_strategy>` -- Executes tasks in foo
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
+* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
 * :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
 * :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\
```

#### html2text {}

```diff
@@ -24,24 +24,26 @@
 ns2.col.foo_cache>` -- Foo files \ :ansopt:`ns2.col.foo#cache:bar`\ Callback
 Plugins ~~~~~~~~~~~~~~~~ * :ref:`foo callback
 ns2.col.foo_callback>` -- Foo output \ :ansopt:`ns2.col.foo#callback:bar`\
 Cliconf Plugins ~~~~~~~~~~~~~~~ * :ref:`foo cliconf
 ns2.col.foo_cliconf>` -- Foo router CLI config Connection Plugins
 ~~~~~~~~~~~~~~~~~~ * :ref:`foo connection
 ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
-bar`\ Filter Plugins ~~~~~~~~~~~~~~ * :ref:`foo filter
+bar`\ Filter Plugins ~~~~~~~~~~~~~~ * :ref:`bar filter
+ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
 ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\
 Inventory Plugins ~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
 ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
 bar`\ Lookup Plugins ~~~~~~~~~~~~~~ * :ref:`foo lookup
 ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\
 Shell Plugins ~~~~~~~~~~~~~ * :ref:`foo shell
 ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ Strategy
 Plugins ~~~~~~~~~~~~~~~~ * :ref:`foo strategy
 ns2.col.foo_strategy>` -- Executes tasks in foo Test Plugins ~~~~~~~~~~~~ * :
-ref:`foo test
+ref:`bar test
+ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
 ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ Vars
 Plugins ~~~~~~~~~~~~ * :ref:`foo vars
 ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ Role Index ---
 ------- These are the roles in the ns2.col collection: * :ref:`foo role
 ns2.col.foo_role>` -- Foo role .. seealso:: List of :ref:`collections ` with
 docs hosted here.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst`

 * *Files 7% similar despite different names*

```diff
@@ -173,27 +173,33 @@
 
         </div>
 
   * - .. raw:: html
 
         <div class="ansible-option-cell">
         <div class="ansibleOptionAnchor" id="parameter-subfoo"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subbaz"></div>
 
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz:
       .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo:
 
       .. rst-class:: ansible-option-title
 
       **subfoo**
 
       .. raw:: html
 
         <a class="ansibleOptionLink" href="#parameter-subfoo" title="Permalink to this option"></a>
 
       .. rst-class:: ansible-option-type-line
 
+      :ansible-option-aliases:`aliases: subbaz`
+
+      .. rst-class:: ansible-option-type-line
+
       :ansible-option-type:`dictionary`
 
       :ansible-option-versionadded:`added in ns2.flatcol 2.0.0`
 
 
       .. raw:: html
 
@@ -210,27 +216,37 @@
 
         </div>
     
   * - .. raw:: html
 
         <div class="ansible-option-indent"></div><div class="ansible-option-cell">
         <div class="ansibleOptionAnchor" id="parameter-subfoo/foo"></div>
-
+        <div class="ansibleOptionAnchor" id="parameter-subbaz/foo"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subfoo/bam"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subbaz/bam"></div>
+
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz/bam:
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz/foo:
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo/bam:
       .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo/foo:
 
       .. rst-class:: ansible-option-title
 
       **foo**
 
       .. raw:: html
 
         <a class="ansibleOptionLink" href="#parameter-subfoo/foo" title="Permalink to this option"></a>
 
       .. rst-class:: ansible-option-type-line
 
+      :ansible-option-aliases:`aliases: bam`
+
+      .. rst-class:: ansible-option-type-line
+
       :ansible-option-type:`string` / :ansible-option-required:`required`
 
       .. raw:: html
 
         </div>
 
     - .. raw:: html
@@ -239,14 +255,18 @@
 
       A sub foo.
 
       Whatever.
 
       Also required when \ :ansopt:`ns2.flatcol.foo#module:subfoo`\  is specified when \ :ansopt:`ns2.flatcol.foo#module:foo=bar`\  or \ :ansval:`baz`\ .
 
+      Note that \ :ansopt:`ns2.flatcol.foo#module:subfoo.foo`\  is the same as \ :ansopt:`ns2.flatcol.foo#module:subbaz.foo`\ , \ :ansopt:`ns2.flatcol.foo#module:subbaz.bam`\ , and \ :ansopt:`ns2.flatcol.foo#module:subfoo.bam`\ .
+
+      \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
+
 
       .. raw:: html
 
         </div>
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/environment_variables.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. contents::
    :local:
    :depth: 1
 
 .. Deprecated
 
+DEPRECATED
+----------
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 --------
 
 .. Description
 
 - This become plugin uses foo.
@@ -115,16 +126,22 @@
       :ansible-option-versionadded:`added in ns2.col 1.2.0`
 
 
 
       Removed in: version 4.0.0
 
       Why: Just some other text.
+      This one has more than one line though.
+      One more.
+
 
       Alternative: nothing
+      relevant
+      I know of
+
 
 
 
 
       .. raw:: html
 
         </div>
@@ -335,14 +352,23 @@
 
 
 .. Return values
 
 
 ..  Status (Presently only deprecated)
 
+Status
+------
+
+.. Deprecated note
+
+- This become will be removed in version 5.0.0.
+  *[deprecated]*
+- For more information see `DEPRECATED`_.
+
 
 .. Authors
 
 Authors
 ~~~~~~~
 
 - Nobody
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
+- \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. rst-class:: ansible-version-added
 
 New in ns2.col 0.2.0
 
 .. Deprecated
 
+DEPRECATED
+^^^^^^^^^^
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 ^^^^^^^^
 
 .. Description
 
 - This is the foo role.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -146,20 +146,22 @@
 
     foo_connection
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
+* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
 * :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
+    bar_filter
     foo_filter
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
 * :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
@@ -206,20 +208,22 @@
 
     foo_strategy
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
+* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
 * :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
+    bar_test
     foo_test
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
 * :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\
```

#### html2text {}

```diff
@@ -30,30 +30,32 @@
 toctree:: :maxdepth: 1 :hidden: foo_callback Cliconf Plugins ~~~~~~~~~~~~~~~ *
 :ref:`foo cliconf
 ns2.col.foo_cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :
 hidden: foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ref:`foo
 connection
 ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
 bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins
-~~~~~~~~~~~~~~ * :ref:`foo filter
+~~~~~~~~~~~~~~ * :ref:`bar filter
+ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
 ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_filter Inventory Plugins ~~~~~~~~~~~~~~~~~
-* :ref:`foo inventory
+toctree:: :maxdepth: 1 :hidden: bar_filter foo_filter Inventory Plugins
+~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
 ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
 bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins
 ~~~~~~~~~~~~~~ * :ref:`foo lookup
 ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :ref:
 `foo shell
 ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :
 ref:`foo strategy
 ns2.col.foo_strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :
-hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`foo test
+hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`bar test
+ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
 ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_test Vars Plugins ~~~~~~~~~~~~ * :ref:`foo
-vars
+toctree:: :maxdepth: 1 :hidden: bar_test foo_test Vars Plugins ~~~~~~~~~~~~ * :
+ref:`foo vars
 ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
 maxdepth: 1 :hidden: foo_vars Role Index ---------- These are the roles in the
 ns2.col collection: * :ref:`foo role
 ns2.col.foo_role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
 seealso:: List of :ref:`collections ` with docs hosted here.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst`

 * *Files 7% similar despite different names*

```diff
@@ -173,27 +173,33 @@
 
         </div>
 
   * - .. raw:: html
 
         <div class="ansible-option-cell">
         <div class="ansibleOptionAnchor" id="parameter-subfoo"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subbaz"></div>
 
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz:
       .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo:
 
       .. rst-class:: ansible-option-title
 
       **subfoo**
 
       .. raw:: html
 
         <a class="ansibleOptionLink" href="#parameter-subfoo" title="Permalink to this option"></a>
 
       .. rst-class:: ansible-option-type-line
 
+      :ansible-option-aliases:`aliases: subbaz`
+
+      .. rst-class:: ansible-option-type-line
+
       :ansible-option-type:`dictionary`
 
       :ansible-option-versionadded:`added in ns2.flatcol 2.0.0`
 
 
       .. raw:: html
 
@@ -210,27 +216,37 @@
 
         </div>
     
   * - .. raw:: html
 
         <div class="ansible-option-indent"></div><div class="ansible-option-cell">
         <div class="ansibleOptionAnchor" id="parameter-subfoo/foo"></div>
-
+        <div class="ansibleOptionAnchor" id="parameter-subbaz/foo"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subfoo/bam"></div>
+        <div class="ansibleOptionAnchor" id="parameter-subbaz/bam"></div>
+
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz/bam:
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subbaz/foo:
+      .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo/bam:
       .. _ansible_collections.ns2.flatcol.foo_module__parameter-subfoo/foo:
 
       .. rst-class:: ansible-option-title
 
       **foo**
 
       .. raw:: html
 
         <a class="ansibleOptionLink" href="#parameter-subfoo/foo" title="Permalink to this option"></a>
 
       .. rst-class:: ansible-option-type-line
 
+      :ansible-option-aliases:`aliases: bam`
+
+      .. rst-class:: ansible-option-type-line
+
       :ansible-option-type:`string` / :ansible-option-required:`required`
 
       .. raw:: html
 
         </div>
 
     - .. raw:: html
@@ -239,14 +255,18 @@
 
       A sub foo.
 
       Whatever.
 
       Also required when \ :ansopt:`ns2.flatcol.foo#module:subfoo`\  is specified when \ :ansopt:`ns2.flatcol.foo#module:foo=bar`\  or \ :ansval:`baz`\ .
 
+      Note that \ :ansopt:`ns2.flatcol.foo#module:subfoo.foo`\  is the same as \ :ansopt:`ns2.flatcol.foo#module:subbaz.foo`\ , \ :ansopt:`ns2.flatcol.foo#module:subbaz.bam`\ , and \ :ansopt:`ns2.flatcol.foo#module:subfoo.bam`\ .
+
+      \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
+
 
       .. raw:: html
 
         </div>
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/build.sh` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-collections/conf.py` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-collections/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/build.sh` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-config/conf.py` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-config/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/build.sh` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-current/conf.py` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-current/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/build.sh` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-sphinx-init-extra/conf.py` & `antsibull_docs-2.1.0/tests/functional/baseline-sphinx-init-extra/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/environment_variables.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_become.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_become.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. contents::
    :local:
    :depth: 1
 
 .. Deprecated
 
+DEPRECATED
+----------
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 --------
 
 .. Description
 
 - This become plugin uses foo.
@@ -115,16 +126,22 @@
       :ansible-option-versionadded:`added in ns2.col 1.2.0`
 
 
 
       Removed in: version 4.0.0
 
       Why: Just some other text.
+      This one has more than one line though.
+      One more.
+
 
       Alternative: nothing
+      relevant
+      I know of
+
 
 
 
 
       .. raw:: html
 
         </div>
@@ -335,14 +352,23 @@
 
 
 .. Return values
 
 
 ..  Status (Presently only deprecated)
 
+Status
+------
+
+.. Deprecated note
+
+- This become will be removed in version 5.0.0.
+  *[deprecated]*
+- For more information see `DEPRECATED`_.
+
 
 .. Authors
 
 Authors
 ~~~~~~~
 
 - Nobody
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_cache.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_callback.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_connection.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_filter.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_inventory.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_lookup.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_module.rst`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
+- \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_role.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_role.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. rst-class:: ansible-version-added
 
 New in ns2.col 0.2.0
 
 .. Deprecated
 
+DEPRECATED
+^^^^^^^^^^
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 ^^^^^^^^
 
 .. Description
 
 - This is the foo role.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_shell.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_strategy.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_test.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/foo_vars.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -146,20 +146,22 @@
 
     foo_connection
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
+* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
 * :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
+    bar_filter
     foo_filter
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
 * :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
@@ -206,20 +208,22 @@
 
     foo_strategy
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
+* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
 * :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
+    bar_test
     foo_test
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
 * :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\
```

#### html2text {}

```diff
@@ -30,29 +30,31 @@
 toctree:: :maxdepth: 1 :hidden: foo_callback Cliconf Plugins ~~~~~~~~~~~~~~~ *
 :ref:`foo cliconf
 ns2.col.foo_cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :
 hidden: foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ref:`foo
 connection
 ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
 bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins
-~~~~~~~~~~~~~~ * :ref:`foo filter
+~~~~~~~~~~~~~~ * :ref:`bar filter
+ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
 ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_filter Inventory Plugins ~~~~~~~~~~~~~~~~~
-* :ref:`foo inventory
+toctree:: :maxdepth: 1 :hidden: bar_filter foo_filter Inventory Plugins
+~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
 ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
 bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins
 ~~~~~~~~~~~~~~ * :ref:`foo lookup
 ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :ref:
 `foo shell
 ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :
 ref:`foo strategy
 ns2.col.foo_strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :
-hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`foo test
+hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`bar test
+ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
 ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_test Vars Plugins ~~~~~~~~~~~~ * :ref:`foo
-vars
+toctree:: :maxdepth: 1 :hidden: bar_test foo_test Vars Plugins ~~~~~~~~~~~~ * :
+ref:`foo vars
 ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
 maxdepth: 1 :hidden: foo_vars Role Index ---------- These are the roles in the
 ns2.col collection: * :ref:`foo role
 ns2.col.foo_role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst`

 * *Files 11% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. contents::
    :local:
    :depth: 1
 
 .. Deprecated
 
+DEPRECATED
+----------
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 --------
 
 .. Description
 
 - This become plugin uses foo.
@@ -99,16 +110,22 @@
       <p class="ansible-option-title"><strong>bar</strong></p>
       <a class="ansibleOptionLink" href="#parameter-bar" title="Permalink to this option"></a>
       <p class="ansible-option-type-line">
         <span class="ansible-option-type">string</span>
       </p>
       <p><span class="ansible-option-versionadded">added in ns2.col 1.2.0</span></p>
   <p>Removed in: version 4.0.0</p>
-  <p>Why: Just some other text.</p>
-  <p>Alternative: nothing</p>
+  <p>Why: Just some other text.
+  This one has more than one line though.
+  One more.
+  </p>
+  <p>Alternative: nothing
+  relevant
+  I know of
+  </p>
 
     </div></td>
     <td><div class="ansible-option-cell">
       <p>Bar. <b>BAR!</b></p>
       <p>Totally unrelated to <code class="ansible-option literal notranslate"><strong><a class="reference internal" href="#parameter-become_user"><span class="std std-ref"><span class="pre">become_user</span></span></a></strong></code>. Even with <code class="ansible-option-value literal notranslate"><a class="reference internal" href="#parameter-become_user"><span class="std std-ref"><span class="pre">become_user=foo</span></span></a></code>.</p>
       <p>Might not be compatible when <code class="ansible-option literal notranslate"><strong><a class="reference internal" href="#parameter-become_user"><span class="std std-ref"><span class="pre">become_user</span></span></a></strong></code> is <code class="ansible-value literal notranslate">bar</code>, though.</p>
     </div></td>
@@ -243,14 +260,23 @@
 
 
 .. Return values
 
 
 ..  Status (Presently only deprecated)
 
+Status
+------
+
+.. Deprecated note
+
+- This become will be removed in version 5.0.0.
+  *[deprecated]*
+- For more information see `DEPRECATED`_.
+
 
 .. Authors
 
 Authors
 ~~~~~~~
 
 - Nobody
```

#### html2text {}

```diff
@@ -16,64 +16,73 @@
 ansible.builtin .. Anchors: aliases .. Title ns2.col.foo become -- Use foo \ :
 ansopt:`ns2.col.foo#become:bar`\
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ ..
 Collection note .. note:: This become plugin is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. version_added .. contents:: :local: :depth: 1 ..
-Deprecated Synopsis -------- .. Description - This become plugin uses foo. -
-This is a second paragraph. .. Aliases .. Requirements .. Options Parameters --
--------- .. raw:: html
-Parameter                  Comments
-bar                        Bar. BAR!
-string                     Totally unrelated to become_user. Even with
-added in ns2.col 1.2.0     become_user=foo.
-Removed in: version 4.0.0  Might not be compatible when become_user is bar,
-Why: Just some other text. though.
-Alternative: nothing
-                           Foo executable.
-                           Default: "foo"
-                           Configuration:
-                               * INI entries
-                                 [privilege_escalation]
-                                   become_exe = foo
-                                 [foo_become_plugin]
-                                   executable = foo
-                                 Removed in: version 3.0.0
-become_exe                       Why: Just some text.
-string                           Alternative: nothing
-added in ns2.col 0.2.0         * Environment variable: ANSIBLE_BECOME_EXE
-                               * Environment variable: ANSIBLE_FOO_EXE
-                                 Removed in: version 3.0.0
-                                 Why: Just some text.
-                                 Alternative: nothing
-                               * Variable: ansible_become_exe
-                               * Variable: ansible_foo_exe
-                                 Removed in: version 3.0.0
-                                 Why: Just some text.
-                                 Alternative: nothing
-                               * Keyword: become_exe
-                           User you &#x27;become&#x27; to execute the task.
-                           Default: "root"
-                           Configuration:
-                               * INI entries
-                                 [privilege_escalation]
-                                   become_user = root
-                                 added in ns2.col 0.1.0
-become_user                      [foo_become_plugin]
-string                             user = root
-                               * Environment variable: ANSIBLE_BECOME_USER
-                                 added in ns2.col 0.1.0
-                               * Environment variable: ANSIBLE_FOO_USER
-                               * Variable: ansible_become_user
-                               * Variable: ansible_foo_user
-                                 added in ns2.col 0.1.0
-                               * Keyword: become_user
-                                 added in ns2.col 0.1.0
+Deprecated DEPRECATED ---------- :Removed in: version 5.0.0 :Why: Just some
+text. This one has more than one line. And one more. :Alternative: I don't know
+of any alternative. Synopsis -------- .. Description - This become plugin uses
+foo. - This is a second paragraph. .. Aliases .. Requirements .. Options
+Parameters ---------- .. raw:: html
+Parameter                               Comments
+bar
+string                                  Bar. BAR!
+added in ns2.col 1.2.0                  Totally unrelated to become_user. Even
+Removed in: version 4.0.0               with become_user=foo.
+Why: Just some other text. This one has Might not be compatible when
+more than one line though. One more.    become_user is bar, though.
+Alternative: nothing relevant I know of
+                                        Foo executable.
+                                        Default: "foo"
+                                        Configuration:
+                                            * INI entries
+                                              [privilege_escalation]
+                                                become_exe = foo
+                                              [foo_become_plugin]
+                                                executable = foo
+                                              Removed in: version 3.0.0
+                                              Why: Just some text.
+become_exe                                    Alternative: nothing
+string                                      * Environment variable:
+added in ns2.col 0.2.0                        ANSIBLE_BECOME_EXE
+                                            * Environment variable:
+                                              ANSIBLE_FOO_EXE
+                                              Removed in: version 3.0.0
+                                              Why: Just some text.
+                                              Alternative: nothing
+                                            * Variable: ansible_become_exe
+                                            * Variable: ansible_foo_exe
+                                              Removed in: version 3.0.0
+                                              Why: Just some text.
+                                              Alternative: nothing
+                                            * Keyword: become_exe
+                                        User you &#x27;become&#x27; to execute
+                                        the task.
+                                        Default: "root"
+                                        Configuration:
+                                            * INI entries
+                                              [privilege_escalation]
+                                                become_user = root
+                                              added in ns2.col 0.1.0
+                                              [foo_become_plugin]
+become_user                                     user = root
+string                                      * Environment variable:
+                                              ANSIBLE_BECOME_USER
+                                              added in ns2.col 0.1.0
+                                            * Environment variable:
+                                              ANSIBLE_FOO_USER
+                                            * Variable: ansible_become_user
+                                            * Variable: ansible_foo_user
+                                              added in ns2.col 0.1.0
+                                            * Keyword: become_user
+                                              added in ns2.col 0.1.0
 .. Attributes .. Notes .. Seealso .. Examples .. Facts .. Return values ..
-Status (Presently only deprecated) .. Authors Authors ~~~~~~~ - Nobody ..
-hint:: Configuration entries for each entry type have a low to high priority
-order. For example, a variable that is lower in the list will override a
-variable that is higher up. .. Extra links Collection links ~~~~~~~~~~~~~~~~ ..
-raw:: html
+Status (Presently only deprecated) Status ------ .. Deprecated note - This
+become will be removed in version 5.0.0. *[deprecated]* - For more information
+see `DEPRECATED`_. .. Authors Authors ~~~~~~~ - Nobody .. hint:: Configuration
+entries for each entry type have a low to high priority order. For example, a
+variable that is lower in the list will override a variable that is higher up.
+.. Extra links Collection links ~~~~~~~~~~~~~~~~ .. raw:: html
 Issue_Tracker Homepage Repository_(Sources) Submit_a_bug_report Communication
 .. Parsing errors
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 Synopsis
 --------
 
 .. Description
 
 - Does some foo on the remote host.
 - Whether foo is magic or not has not yet been determined.
+- \ :ansenvvarref:`FOOBAR1`\ , \ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\ .
 
 
 .. Aliases
 
 
 .. Requirements
```

#### html2text {}

```diff
@@ -20,15 +20,17 @@
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it, use: :code:
 `ansible-galaxy collection install ns2.col`. You need further requirements to
 be able to use this module, see :ref:`Requirements
 ns2.col.foo_module_requirements>` for details. To use it in a playbook,
 specify: :code:`ns2.col.foo`. .. version_added .. rst-class:: ansible-version-
 added New in ns2.col 2.0.0 .. contents:: :local: :depth: 1 .. Deprecated
 Synopsis -------- .. Description - Does some foo on the remote host. - Whether
-foo is magic or not has not yet been determined. .. Aliases .. Requirements ..
+foo is magic or not has not yet been determined. - \ :ansenvvarref:`FOOBAR1`\ ,
+\ :ansenvvarref:`FOOBAR2`\ , \ :ansenvvar:`FOOBAR3`\ , \ :ansenvvar:`FOOBAR4`\
+. .. Aliases .. Requirements ..
 _ansible_collections.ns2.col.foo_module_requirements: Requirements -----------
 - The below requirements are needed on the host that executes this module. -
 Foo on remote. .. Options Parameters ---------- .. raw:: html
 Parameter               Comments
 bar                     A bar.
 aliases: baz            Independent from foo.
 list / elements=integer Do not confuse with bar.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,25 @@
 
 .. rst-class:: ansible-version-added
 
 New in ns2.col 0.2.0
 
 .. Deprecated
 
+DEPRECATED
+^^^^^^^^^^
+:Removed in: version 5.0.0
+:Why: Just some text.
+      This one has more than one line.
+      And one more.
+
+:Alternative: I don't know
+              of any
+              alternative.
+
 
 Synopsis
 ^^^^^^^^
 
 .. Description
 
 - This is the foo role.
```

#### html2text {}

```diff
@@ -14,19 +14,21 @@
 _ansible_collections.ns2.col.foo_role: .. Anchors: aliases .. Title ns2.col.foo
 role -- Foo role ++++++++++++++++++++++++++++ .. Collection note .. note:: This
 role is part of the `ns2.col collection
 galaxy.ansible.com/ns2/col>`_ (version 2.1.0). To install it use: :code:
 `ansible-galaxy collection install ns2.col`. To use it in a playbook, specify:
 :code:`ns2.col.foo`. .. contents:: :local: :depth: 2 .. Entry point title Entry
 point ``main`` -- Foo role -------------------------------- .. version_added ..
-rst-class:: ansible-version-added New in ns2.col 0.2.0 .. Deprecated Synopsis
-^^^^^^^^ .. Description - This is the foo role. - If you set \ :ansopt:
-`ns2.col.foo#role:main:foo\_param\_1`\ while \ :ansopt:`ns2.col.foo#role:main:
-foo\_param\_2=3`\ , this might behave funny. .. Requirements .. Options
-Parameters ^^^^^^^^^^ .. raw:: html
+rst-class:: ansible-version-added New in ns2.col 0.2.0 .. Deprecated DEPRECATED
+^^^^^^^^^^ :Removed in: version 5.0.0 :Why: Just some text. This one has more
+than one line. And one more. :Alternative: I don't know of any alternative.
+Synopsis ^^^^^^^^ .. Description - This is the foo role. - If you set \ :
+ansopt:`ns2.col.foo#role:main:foo\_param\_1`\ while \ :ansopt:
+`ns2.col.foo#role:main:foo\_param\_2=3`\ , this might behave funny. ..
+Requirements .. Options Parameters ^^^^^^^^^^ .. raw:: html
 Parameter   Comments
 foo_param_1 A string parameter
 string      If you set foo_param_1 while foo_param_2=3, this might behave
             funny.
 foo_param_2 An integer parameter with a default.
 integer     Default: 13
 .. Attributes Attributes ---------- .. rst-class:: ansible-option-table ..
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -146,20 +146,22 @@
 
     foo_connection
 
 
 Filter Plugins
 ~~~~~~~~~~~~~~
 
+* :ref:`bar filter <ansible_collections.ns2.col.bar_filter>` -- The bar filter
 * :ref:`foo filter <ansible_collections.ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
+    bar_filter
     foo_filter
 
 
 Inventory Plugins
 ~~~~~~~~~~~~~~~~~
 
 * :ref:`foo inventory <ansible_collections.ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:bar`\ 
@@ -206,20 +208,22 @@
 
     foo_strategy
 
 
 Test Plugins
 ~~~~~~~~~~~~
 
+* :ref:`bar test <ansible_collections.ns2.col.bar_test>` -- Is something a bar
 * :ref:`foo test <ansible_collections.ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ 
 
 .. toctree::
     :maxdepth: 1
     :hidden:
 
+    bar_test
     foo_test
 
 
 Vars Plugins
 ~~~~~~~~~~~~
 
 * :ref:`foo vars <ansible_collections.ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\
```

#### html2text {}

```diff
@@ -30,30 +30,32 @@
 toctree:: :maxdepth: 1 :hidden: foo_callback Cliconf Plugins ~~~~~~~~~~~~~~~ *
 :ref:`foo cliconf
 ns2.col.foo_cliconf>` -- Foo router CLI config .. toctree:: :maxdepth: 1 :
 hidden: foo_cliconf Connection Plugins ~~~~~~~~~~~~~~~~~~ * :ref:`foo
 connection
 ns2.col.foo_connection>` -- Foo connection \ :ansopt:`ns2.col.foo#connection:
 bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_connection Filter Plugins
-~~~~~~~~~~~~~~ * :ref:`foo filter
+~~~~~~~~~~~~~~ * :ref:`bar filter
+ns2.col.bar_filter>` -- The bar filter * :ref:`foo filter
 ns2.col.foo_filter>` -- The foo filter \ :ansopt:`ns2.col.foo#filter:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_filter Inventory Plugins ~~~~~~~~~~~~~~~~~
-* :ref:`foo inventory
+toctree:: :maxdepth: 1 :hidden: bar_filter foo_filter Inventory Plugins
+~~~~~~~~~~~~~~~~~ * :ref:`foo inventory
 ns2.col.foo_inventory>` -- The foo inventory \ :ansopt:`ns2.col.foo#inventory:
 bar`\ .. toctree:: :maxdepth: 1 :hidden: foo_inventory Lookup Plugins
 ~~~~~~~~~~~~~~ * :ref:`foo lookup
 ns2.col.foo_lookup>` -- Look up some foo \ :ansopt:`ns2.col.foo#lookup:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_lookup Shell Plugins ~~~~~~~~~~~~~ * :ref:
 `foo shell
 ns2.col.foo_shell>` -- Foo shell \ :ansopt:`ns2.col.foo#shell:bar`\ ..
 toctree:: :maxdepth: 1 :hidden: foo_shell Strategy Plugins ~~~~~~~~~~~~~~~~ * :
 ref:`foo strategy
 ns2.col.foo_strategy>` -- Executes tasks in foo .. toctree:: :maxdepth: 1 :
-hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`foo test
+hidden: foo_strategy Test Plugins ~~~~~~~~~~~~ * :ref:`bar test
+ns2.col.bar_test>` -- Is something a bar * :ref:`foo test
 ns2.col.foo_test>` -- Is something a foo \ :ansopt:`ns2.col.foo#test:bar`\ ..
-toctree:: :maxdepth: 1 :hidden: foo_test Vars Plugins ~~~~~~~~~~~~ * :ref:`foo
-vars
+toctree:: :maxdepth: 1 :hidden: bar_test foo_test Vars Plugins ~~~~~~~~~~~~ * :
+ref:`foo vars
 ns2.col.foo_vars>` -- Load foo \ :ansopt:`ns2.col.foo#vars:bar`\ .. toctree:: :
 maxdepth: 1 :hidden: foo_vars Role Index ---------- These are the roles in the
 ns2.col collection: * :ref:`foo role
 ns2.col.foo_role>` -- Foo role .. toctree:: :maxdepth: 1 :hidden: foo_role ..
 seealso:: List of :ref:`collections ` with docs hosted here.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.1.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,24 @@
     name: foo
     short_description: Use foo O(bar)
     description:
         - This become plugin uses foo.
         - This is a second paragraph.
     author: Nobody (!UNKNOWN)
     version_added: historical
+    deprecated:
+        removed_in: 5.0.0
+        why: |
+          Just some text.
+          This one has more than one line.
+          And one more.
+        alternatives: |
+          I don't know
+          of any
+          alternative.
     options:
         become_user:
             description: User you 'become' to execute the task.
             default: root
             ini:
               - section: privilege_escalation
                 key: become_user
@@ -68,17 +78,23 @@
             description:
                 - Bar. B(BAR!)
                 - Totally unrelated to O(become_user). Even with O(become_user=foo).
                 - Might not be compatible when O(become_user) is V(bar), though.
             type: str
             version_added: 1.2.0
             deprecated:
-                why: Just some other text.
+                why: |
+                  Just some other text.
+                  This one has more than one line though.
+                  One more.
                 version: 4.0.0
-                alternatives: nothing
+                alternatives: |
+                  nothing
+                  relevant
+                  I know of
 """
 
 from ansible.plugins.become import BecomeBase
 
 
 class BecomeModule(BecomeBase):
     name = "ns2.col.foo"
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,17 +39,12 @@
 """
 
 
 def foo(input, foo):
     return "FOO:{0}:BAR".format(input)
 
 
-def bar(input, foo, bar, baz):
-    return input | foo
-
-
 class FilterModule(object):
     def filters(self):
         return {
             "foo": foo,
-            "bar": bar,
         }
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     - "Ansible Core Team"
     - "Someone else (@ansible)"
 version_added: "2.0.0"
 short_description: Do some foo O(bar)
 description:
     - Does some foo on the remote host.
     - Whether foo is magic or not has not yet been determined.
+    - E(FOOBAR1), E(FOOBAR2), E(FOOBAR3), E(FOOBAR4).
 options:
     foo:
         description: The foo source.
         type: str
         required: true
     bar:
         description:
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,18 +34,12 @@
 """
 
 
 def foo(input):
     return True
 
 
-def bar(input):
-    return False
-
-
 class TestModule(object):
     def tests(self):
         return {
             "foo": foo,
-            "bar": bar,
-            "is_bar": bar,
         }
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -24,7 +24,17 @@
         default: 13
     attributes:
       check_mode:
         description: Can run in check_mode and return changed status prediction without modifying target
         support: full
     seealso:
       - module: ns2.col.foo
+    deprecated:
+        removed_in: 5.0.0
+        why: |
+          Just some text.
+          This one has more than one line.
+          And one more.
+        alternatives: |
+          I don't know
+          of any
+          alternative.
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,22 +33,28 @@
         elements: int
         aliases:
           - baz
     subfoo:
         description: Some recursive foo.
         version_added: 2.0.0
         type: dict
+        aliases:
+          - subbaz
         suboptions:
             foo:
                 description:
                     - A sub foo.
                     - Whatever.
                     - Also required when O(subfoo) is specified when O(foo=bar) or V(baz).
+                    - Note that O(subfoo.foo) is the same as O(subbaz.foo), O(subbaz.bam), and O(subfoo.bam).
+                    - E(FOOBAR1), E(FOOBAR2), E(FOOBAR3), E(FOOBAR4).
                 type: str
                 required: true
+                aliases:
+                  - bam
 """
 
 EXAMPLES = """
 - name: Do some foo
   ns2.flatcol.foo:
     foo: '{{ foo }}'
     bar:
@@ -74,15 +80,21 @@
 
 
 def main():
     module = AnsibleModule(
         argument_spec=dict(
             foo=dict(type="str", required=True),
             bar=dict(type="list", elements="int", aliases=["baz"]),
-            subfoo=dict(type="dict", options=dict(foo=dict(type="str", required=True))),
+            subfoo=dict(
+                type="dict",
+                aliases=["subbaz"],
+                options=dict(
+                    foo=dict(type="str", required=True, aliases=["bam"]),
+                ),
+            ),
         ),
         supports_check_mode=True,
     )
     module.exit_json(bar="baz")
 
 
 if __name__ == "__main__":
```

### Comparing `antsibull_docs-2.0.0a2/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py` & `antsibull_docs-2.1.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/test_schema.py` & `antsibull_docs-2.1.0/tests/functional/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_become.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_become.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_become_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_become_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cache.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cache.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cache_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cache_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_callback.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_callback.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_callback_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_callback_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cliconf.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cliconf.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_cliconf_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_cliconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_connection.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_connection_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_filter.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_filter.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_filter_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_filter_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_httpapi.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_httpapi.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_httpapi_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_httpapi_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_inventory.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_inventory.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_inventory_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_inventory_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_lookup.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_lookup.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_lookup_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_lookup_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_module.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_module.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_module_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_module_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_netconf.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_netconf.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_netconf_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_netconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_role.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_role.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_role_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_role_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_shell.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_shell.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_shell_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_shell_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_strategy.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_strategy.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_strategy_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_strategy_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_test.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_test.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_test_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_test_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_vars.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_vars.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/one_vars_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/one_vars_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/ssh_connection.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/ssh_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/functional/schema/good_data/ssh_connection_results.json` & `antsibull_docs-2.1.0/tests/functional/schema/good_data/ssh_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/units/test_jinja2.py` & `antsibull_docs-2.1.0/tests/units/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/units/markup/test_counter.py` & `antsibull_docs-2.1.0/tests/units/markup/test_counter.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/tests/units/markup/test_markup.py` & `antsibull_docs-2.1.0/tests/units/markup/test_markup.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/.gitignore` & `antsibull_docs-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/README.md` & `antsibull_docs-2.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,19 @@
 
 antsibull-docs is covered by the [Ansible Code of Conduct](https://docs.ansible.com/ansible/latest/community/code_of_conduct.html).
 
 ## Versioning and compatibility
 
 From version 1.0.0 on, antsibull-docs sticks to semantic versioning and aims at providing no backwards compatibility breaking changes **to the command line API (antsibull-docs)** during a major release cycle. We might make exceptions from this in case of security fixes for vulnerabilities that are severe enough.
 
-We explicitly exclude code compatibility. **antsibull-docs is not supposed to be used as a library.** The only exception are dependencies with other antsibull projects (currently, only [antsibull](https://github.com/ansible-community/antsibull/) itself). If you want to use a certain part of antsibull-docs as a library, please create an issue so we can discuss whether we add a stable interface for **parts** of the Python code. We do not promise that this will actually happen though.
+The current major version is 2.x.y. Development for 2.x.y occurs on the `main` branch. 2.x.y mainly differs from 1.x.y by dropping support for Python 3.6, 3.7, and 3.8, and by dropping support for older Ansible/ansible-base/ansible-core versions. See the changelog for details. 1.x.y is still developed on the `stable-1` branch, but only security fixes, major bugfixes, and other absolutely necessary changes will be backported.
+
+We explicitly exclude code compatibility. **antsibull-docs is not supposed to be used as a library.** The only exception are potential dependencies with other antsibull projects (currently there are none). If you want to use a certain part of antsibull-docs as a library, please create an issue so we can discuss whether we add a stable interface for **parts** of the Python code. We do not promise that this will actually happen though.
+
+If you are interested in library support for interpreting Ansible markup, please take a look at [the antsibull-docs-parser project](https://github.com/ansible-community/antsibull-docs-parser).
 
 ## Using the Sphinx extension
 
 Include it in your Sphinx configuration ``conf.py``::
 
 ```
 # Add it to 'extensions':
```

### Comparing `antsibull_docs-2.0.0a2/pyproject.toml` & `antsibull_docs-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "antsibull-docs"
-version = "2.0.0a2"
+version = "2.1.0"
 description = "Tools for building Ansible documentation"
 license = "GPL-3.0-or-later"
 license-files = {globs=["LICENSES/*.txt"]}
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Ansible",
```

### Comparing `antsibull_docs-2.0.0a2/LICENSES/BSD-2-Clause.txt` & `antsibull_docs-2.1.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.0.0a2/PKG-INFO` & `antsibull_docs-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antsibull-docs
-Version: 2.0.0a2
+Version: 2.1.0
 Summary: Tools for building Ansible documentation
 Project-URL: Source code, https://github.com/ansible-community/antsibull-docs
 Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
 Project-URL: Bug tracker, https://github.com/ansible-community/antsibull-docs/issues
 Author-email: Toshio Kuratomi <a.badger@gmail.com>, Felix Fontein <felix@fontein.de>
 Maintainer-email: Felix Fontein <felix@fontein.de>, Maxwell G <maxwell@gtmx.me>
 License-Expression: GPL-3.0-or-later
@@ -92,15 +92,19 @@
 
 antsibull-docs is covered by the [Ansible Code of Conduct](https://docs.ansible.com/ansible/latest/community/code_of_conduct.html).
 
 ## Versioning and compatibility
 
 From version 1.0.0 on, antsibull-docs sticks to semantic versioning and aims at providing no backwards compatibility breaking changes **to the command line API (antsibull-docs)** during a major release cycle. We might make exceptions from this in case of security fixes for vulnerabilities that are severe enough.
 
-We explicitly exclude code compatibility. **antsibull-docs is not supposed to be used as a library.** The only exception are dependencies with other antsibull projects (currently, only [antsibull](https://github.com/ansible-community/antsibull/) itself). If you want to use a certain part of antsibull-docs as a library, please create an issue so we can discuss whether we add a stable interface for **parts** of the Python code. We do not promise that this will actually happen though.
+The current major version is 2.x.y. Development for 2.x.y occurs on the `main` branch. 2.x.y mainly differs from 1.x.y by dropping support for Python 3.6, 3.7, and 3.8, and by dropping support for older Ansible/ansible-base/ansible-core versions. See the changelog for details. 1.x.y is still developed on the `stable-1` branch, but only security fixes, major bugfixes, and other absolutely necessary changes will be backported.
+
+We explicitly exclude code compatibility. **antsibull-docs is not supposed to be used as a library.** The only exception are potential dependencies with other antsibull projects (currently there are none). If you want to use a certain part of antsibull-docs as a library, please create an issue so we can discuss whether we add a stable interface for **parts** of the Python code. We do not promise that this will actually happen though.
+
+If you are interested in library support for interpreting Ansible markup, please take a look at [the antsibull-docs-parser project](https://github.com/ansible-community/antsibull-docs-parser).
 
 ## Using the Sphinx extension
 
 Include it in your Sphinx configuration ``conf.py``::
 
 ```
 # Add it to 'extensions':
```

