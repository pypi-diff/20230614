# Comparing `tmp/ersilia-0.1.8.tar.gz` & `tmp/ersilia-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ersilia-0.1.8.tar", last modified: Mon May 15 11:09:11 2023, max compression
+gzip compressed data, was "dist/ersilia-0.1.9.tar", last modified: Mon May 15 14:37:34 2023, max compression
```

## Comparing `ersilia-0.1.8.tar` & `ersilia-0.1.9.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 11:08:58.000000 ersilia-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-15 11:09:11.000000 ersilia-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-15 11:08:58.000000 ersilia-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 11:09:10.000000 ersilia-0.1.8/ersilia/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/app/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/app/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/app/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/app/blocks/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/close.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/cli/commands/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/create_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/db/disk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/disk/fetched.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/db/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/environments/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/environments/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/db/hubdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/localslugs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/bundle/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/bundle/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/bundle/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/slug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/table_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/delete/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/inform.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/lake.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/modify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/sniff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/toolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/fetch/pack/
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/pack/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/pack/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/pure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/io/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/readers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/readers/pyinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/io/types/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/io/types/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)   461883 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/compound.tsv
--rw-r--r--   0 runner    (1001) docker     (123)  2622625 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/protein.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/protein.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/lake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/lake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/lake/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/lake/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/lake/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/publish/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/dockerhub.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/lake.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/serve/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/autoservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/setup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/baseconda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/basedocker.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/setup/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/bentoml.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/eospath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/isaura.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/ping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/setup/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/utils/clone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/cli_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/card_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/catalog_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/clear_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/close_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/delete_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/example_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/fetch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/handle_undecorated_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/issue_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/serve_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/setup_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/throw_ersilia_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/utils/identifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/long.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/short.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/import.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/installers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/utils/supp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/supp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/supp/conda_env_resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:09:11.000000 ersilia-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-15 11:08:58.000000 ersilia-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 11:08:58.000000 ersilia-0.1.8/test/test_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-15 11:08:58.000000 ersilia-0.1.8/test/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-15 11:08:58.000000 ersilia-0.1.8/test/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 14:37:18.000000 ersilia-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-15 14:37:34.000000 ersilia-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-15 14:37:18.000000 ersilia-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 14:37:33.000000 ersilia-0.1.9/ersilia/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/app/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/app/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/app/blocks/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/cli/commands/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/commands/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/create_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/cli/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/core/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/core/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/db/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/disk/fetched.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/db/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/environments/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/environments/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/db/hubdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/hubdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/hubdata/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/hubdata/localslugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/hubdata/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/db/hubdata/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/hub/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/bundle/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/bundle/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/bundle/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/hub/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/content/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/content/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/content/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/content/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/content/slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/content/table_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/hub/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/delete/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/hub/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/inform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/lake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/sniff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/actions/toolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/hub/fetch/pack/
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/pack/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/hub/fetch/pack/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/pure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/io/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/readers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/readers/pyinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/io/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/io/types/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/examples/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)   461883 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/examples/compound.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)  2622625 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/examples/protein.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/io/types/protein.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/lake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/lake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/lake/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/lake/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/lake/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/dockerhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/lake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/publish/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/serve/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/serve/autoservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/serve/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/serve/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/baseconda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/basedocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/setup/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/bentoml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/eospath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/isaura.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/requirements/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/setup/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/setup/utils/clone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/cli_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/card_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/catalog_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/clear_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/close_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/delete_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/example_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/fetch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/handle_undecorated_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/issue_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/serve_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/setup_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/exceptions_utils/throw_ersilia_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/utils/identifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/identifiers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/installers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia/utils/supp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/supp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/supp/conda_env_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 14:37:18.000000 ersilia-0.1.9/ersilia/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 14:37:34.000000 ersilia-0.1.9/ersilia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:37:34.000000 ersilia-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-15 14:37:18.000000 ersilia-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:34.000000 ersilia-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:37:18.000000 ersilia-0.1.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 14:37:18.000000 ersilia-0.1.9/test/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-15 14:37:18.000000 ersilia-0.1.9/test/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-15 14:37:18.000000 ersilia-0.1.9/test/test_models.py
```

### Comparing `ersilia-0.1.8/PKG-INFO` & `ersilia-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersilia
-Version: 0.1.8
+Version: 0.1.9
 Summary: A hub of AI/ML models for open source drug discovery and global health
 Home-page: https://github.com/ersilia-os/ersilia
 Author: Ersilia Open Source Initiative
 Author-email: hello@ersilia.io
 License: GPLv3
 Project-URL: Landing page, https://ersilia.io
 Project-URL: Models, https://ersilia.io/model-hub
```

### Comparing `ersilia-0.1.8/README.md` & `ersilia-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/__init__.py` & `ersilia-0.1.9/ersilia/__init__.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/_version.py` & `ersilia-0.1.9/ersilia/_version.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/app/app.py` & `ersilia-0.1.9/ersilia/app/app.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/app/blocks/streamlit.py` & `ersilia-0.1.9/ersilia/app/blocks/streamlit.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/auth/auth.py` & `ersilia-0.1.9/ersilia/auth/auth.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/cmd.py` & `ersilia-0.1.9/ersilia/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/__init__.py` & `ersilia-0.1.9/ersilia/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/api.py` & `ersilia-0.1.9/ersilia/cli/commands/api.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/card.py` & `ersilia-0.1.9/ersilia/cli/commands/card.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/catalog.py` & `ersilia-0.1.9/ersilia/cli/commands/catalog.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/close.py` & `ersilia-0.1.9/ersilia/cli/commands/close.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/delete.py` & `ersilia-0.1.9/ersilia/cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/deploy.py` & `ersilia-0.1.9/ersilia/cli/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/example.py` & `ersilia-0.1.9/ersilia/cli/commands/example.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/fetch.py` & `ersilia-0.1.9/ersilia/cli/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/info.py` & `ersilia-0.1.9/ersilia/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/publish.py` & `ersilia-0.1.9/ersilia/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/sample.py` & `ersilia-0.1.9/ersilia/cli/commands/sample.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/serve.py` & `ersilia-0.1.9/ersilia/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/setup.py` & `ersilia-0.1.9/ersilia/cli/commands/setup.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/commands/test.py` & `ersilia-0.1.9/ersilia/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/create_cli.py` & `ersilia-0.1.9/ersilia/cli/create_cli.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/echo.py` & `ersilia-0.1.9/ersilia/cli/echo.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/cli/messages.py` & `ersilia-0.1.9/ersilia/cli/messages.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/core/base.py` & `ersilia-0.1.9/ersilia/core/base.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/core/model.py` & `ersilia-0.1.9/ersilia/core/model.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/core/modelbase.py` & `ersilia-0.1.9/ersilia/core/modelbase.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/core/session.py` & `ersilia-0.1.9/ersilia/core/session.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/db/disk/fetched.py` & `ersilia-0.1.9/ersilia/db/disk/fetched.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/db/environments/localdb.py` & `ersilia-0.1.9/ersilia/db/environments/localdb.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/db/environments/managers.py` & `ersilia-0.1.9/ersilia/db/environments/managers.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/db/hubdata/interfaces.py` & `ersilia-0.1.9/ersilia/db/hubdata/interfaces.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/db/hubdata/localslugs.py` & `ersilia-0.1.9/ersilia/db/hubdata/localslugs.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/db/hubdata/samplers.py` & `ersilia-0.1.9/ersilia/db/hubdata/samplers.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/default.py` & `ersilia-0.1.9/ersilia/default.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/bundle/bundle.py` & `ersilia-0.1.9/ersilia/hub/bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/bundle/repo.py` & `ersilia-0.1.9/ersilia/hub/bundle/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
             text = f.read()
         splitter_string = "Service.__name__"
         text = text.split(splitter_string)
         a = text[0]
         b = text[1]
         a += "    @api(input=JsonInput(), batch=True)\n"
         a += "    def info(self, input=None):\n"
+        a += "        import json\n"
         a += "        data = json.load(open('{0}', 'r'))\n".format(information_file)
         a += "        return [data]\n\n"
         with open(file_name, "w") as f:
             s = a + splitter_string + b
             f.write(s)
 
     def check(self):
```

### Comparing `ersilia-0.1.8/ersilia/hub/bundle/status.py` & `ersilia-0.1.9/ersilia/hub/bundle/status.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/content/card.py` & `ersilia-0.1.9/ersilia/hub/content/card.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/content/catalog.py` & `ersilia-0.1.9/ersilia/hub/content/catalog.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/content/information.py` & `ersilia-0.1.9/ersilia/hub/content/information.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/content/search.py` & `ersilia-0.1.9/ersilia/hub/content/search.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/content/slug.py` & `ersilia-0.1.9/ersilia/hub/content/slug.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/content/table_update.py` & `ersilia-0.1.9/ersilia/hub/content/table_update.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/delete/delete.py` & `ersilia-0.1.9/ersilia/hub/delete/delete.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/content.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/content.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/get.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/get.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/inform.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/inform.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/modify.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/modify.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/pack.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/pack.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/prepare.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/prepare.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/setup.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/setup.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/sniff.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/sniff.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/actions/toolize.py` & `ersilia-0.1.9/ersilia/hub/fetch/actions/toolize.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/fetch.py` & `ersilia-0.1.9/ersilia/hub/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/pack/__init__.py` & `ersilia-0.1.9/ersilia/hub/fetch/pack/__init__.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/pack/mode.py` & `ersilia-0.1.9/ersilia/hub/fetch/pack/mode.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/hub/fetch/pack/runners.py` & `ersilia-0.1.9/ersilia/hub/fetch/pack/runners.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/dataframe.py` & `ersilia-0.1.9/ersilia/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/input.py` & `ersilia-0.1.9/ersilia/io/input.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/output.py` & `ersilia-0.1.9/ersilia/io/output.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/pure.py` & `ersilia-0.1.9/ersilia/io/pure.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/readers/file.py` & `ersilia-0.1.9/ersilia/io/readers/file.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/readers/pyinput.py` & `ersilia-0.1.9/ersilia/io/readers/pyinput.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/shape.py` & `ersilia-0.1.9/ersilia/io/shape.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/types/compound.py` & `ersilia-0.1.9/ersilia/io/types/compound.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/types/examples/compound.py` & `ersilia-0.1.9/ersilia/io/types/examples/compound.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/types/examples/compound.tsv` & `ersilia-0.1.9/ersilia/io/types/examples/compound.tsv`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/io/types/examples/protein.tsv` & `ersilia-0.1.9/ersilia/io/types/examples/protein.tsv`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/lake/base.py` & `ersilia-0.1.9/ersilia/lake/base.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/lake/interface.py` & `ersilia-0.1.9/ersilia/lake/interface.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/lake/manager.py` & `ersilia-0.1.9/ersilia/lake/manager.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/deploy.py` & `ersilia-0.1.9/ersilia/publish/deploy.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/dockerhub.py` & `ersilia-0.1.9/ersilia/publish/dockerhub.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/lake.py` & `ersilia-0.1.9/ersilia/publish/lake.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/metadata.py` & `ersilia-0.1.9/ersilia/publish/metadata.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/publish.py` & `ersilia-0.1.9/ersilia/publish/publish.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/rebase.py` & `ersilia-0.1.9/ersilia/publish/rebase.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/s3.py` & `ersilia-0.1.9/ersilia/publish/s3.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/store.py` & `ersilia-0.1.9/ersilia/publish/store.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/publish/test.py` & `ersilia-0.1.9/ersilia/publish/test.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/serve/api.py` & `ersilia-0.1.9/ersilia/serve/api.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/serve/autoservice.py` & `ersilia-0.1.9/ersilia/serve/autoservice.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/serve/schema.py` & `ersilia-0.1.9/ersilia/serve/schema.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/serve/services.py` & `ersilia-0.1.9/ersilia/serve/services.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/setup/baseconda.py` & `ersilia-0.1.9/ersilia/setup/baseconda.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/setup/basedocker.py` & `ersilia-0.1.9/ersilia/setup/basedocker.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/setup/requirements/bentoml.py` & `ersilia-0.1.9/ersilia/setup/requirements/bentoml.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/setup/requirements/compound.py` & `ersilia-0.1.9/ersilia/setup/requirements/compound.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/setup/requirements/docker.py` & `ersilia-0.1.9/ersilia/setup/requirements/docker.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/setup/requirements/git.py` & `ersilia-0.1.9/ersilia/setup/requirements/git.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/setup/utils/clone.py` & `ersilia-0.1.9/ersilia/setup/utils/clone.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/clear.py` & `ersilia-0.1.9/ersilia/utils/clear.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/conda.py` & `ersilia-0.1.9/ersilia/utils/conda.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/config.py` & `ersilia-0.1.9/ersilia/utils/config.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/cron.py` & `ersilia-0.1.9/ersilia/utils/cron.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/csvfile.py` & `ersilia-0.1.9/ersilia/utils/csvfile.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/docker.py` & `ersilia-0.1.9/ersilia/utils/docker.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/download.py` & `ersilia-0.1.9/ersilia/utils/download.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/dvc.py` & `ersilia-0.1.9/ersilia/utils/dvc.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/exceptions_utils/api_exceptions.py` & `ersilia-0.1.9/ersilia/utils/exceptions_utils/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/exceptions_utils/card_exceptions.py` & `ersilia-0.1.9/ersilia/utils/exceptions_utils/card_exceptions.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/exceptions_utils/exceptions.py` & `ersilia-0.1.9/ersilia/utils/exceptions_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/exceptions_utils/fetch_exceptions.py` & `ersilia-0.1.9/ersilia/utils/exceptions_utils/fetch_exceptions.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/exceptions_utils/handle_undecorated_exception.py` & `ersilia-0.1.9/ersilia/utils/exceptions_utils/handle_undecorated_exception.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/exceptions_utils/issue_reporting.py` & `ersilia-0.1.9/ersilia/utils/exceptions_utils/issue_reporting.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/exceptions_utils/setup_exceptions.py` & `ersilia-0.1.9/ersilia/utils/exceptions_utils/setup_exceptions.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/exceptions_utils/throw_ersilia_exception.py` & `ersilia-0.1.9/ersilia/utils/exceptions_utils/throw_ersilia_exception.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/hdf5.py` & `ersilia-0.1.9/ersilia/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/identifiers/compound.py` & `ersilia-0.1.9/ersilia/utils/identifiers/compound.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/identifiers/file.py` & `ersilia-0.1.9/ersilia/utils/identifiers/file.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/identifiers/long.py` & `ersilia-0.1.9/ersilia/utils/identifiers/long.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/identifiers/model.py` & `ersilia-0.1.9/ersilia/utils/identifiers/model.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/identifiers/protein.py` & `ersilia-0.1.9/ersilia/utils/identifiers/protein.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/identifiers/short.py` & `ersilia-0.1.9/ersilia/utils/identifiers/short.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/installers.py` & `ersilia-0.1.9/ersilia/utils/installers.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/logging.py` & `ersilia-0.1.9/ersilia/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/paths.py` & `ersilia-0.1.9/ersilia/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/ports.py` & `ersilia-0.1.9/ersilia/utils/ports.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/supp/conda_env_resolve.py` & `ersilia-0.1.9/ersilia/utils/supp/conda_env_resolve.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/terminal.py` & `ersilia-0.1.9/ersilia/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/upload.py` & `ersilia-0.1.9/ersilia/utils/upload.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/venv.py` & `ersilia-0.1.9/ersilia/utils/venv.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia/utils/versioning.py` & `ersilia-0.1.9/ersilia/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/ersilia.egg-info/PKG-INFO` & `ersilia-0.1.9/ersilia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersilia
-Version: 0.1.8
+Version: 0.1.9
 Summary: A hub of AI/ML models for open source drug discovery and global health
 Home-page: https://github.com/ersilia-os/ersilia
 Author: Ersilia Open Source Initiative
 Author-email: hello@ersilia.io
 License: GPLv3
 Project-URL: Landing page, https://ersilia.io
 Project-URL: Models, https://ersilia.io/model-hub
```

### Comparing `ersilia-0.1.8/ersilia.egg-info/SOURCES.txt` & `ersilia-0.1.9/ersilia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/setup.py` & `ersilia-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/test/test_inputs.py` & `ersilia-0.1.9/test/test_inputs.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.8/test/test_models.py` & `ersilia-0.1.9/test/test_models.py`

 * *Files identical despite different names*

